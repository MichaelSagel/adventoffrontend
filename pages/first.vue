<template>
  <div class="first">
    
    <BaseTimer :time-left="timeLeft" />

    <div class="baseTimer">
      <svg
        class="baseTimer"
        viewBox="0 0 100 100"
        xmlns="http://www.w3.org/2000/svg"
      >
        <g class="baseTimer">
          <circle
            class="baseTimer__pathElapsed"
            cx="50"
            cy="50"
            r="45"
          ></circle>
          <path
            :stroke-dasharray="circleDasharray"
            class="baseTimer__pathRemaining"
            :class="remainingPathColor"
            d="
            M 50, 50
            m -45, 0
            a 45,45 0 1,0 90,0
            a 45,45 0 1,0 -90,0
          "
          ></path>
        </g>
      </svg>
      <span class="baseTimer__label">{{ formattedTimeLeft }}</span>
    </div>

    <div
      class="startOrStop"
      @click="start"
    >
      <template v-if="isStarted">S T O P</template>
      <template v-else>S T A R T</template>
    </div>
  </div>
</template>

<script>
const FULL_DASH_ARRAY = 283;
const WARNING_THRESHOLD = 10;
const ALERT_THRESHOLD = 5;

const COLOR_CODES = {
  info: {
    color: "green",
  },
  warning: {
    color: "orange",
    threshold: WARNING_THRESHOLD,
  },
  alert: {
    color: "red",
    threshold: ALERT_THRESHOLD,
  },
};

const TIME_LIMIT = 20;

export default {
  colorMode: "first",
  data: function () {
    return {
      isStarted: false,
      timeLimit: 900,
      timePassed: 0,
      timerInterval: null,
    };
  },
  computed: {
    circleDasharray() {
      return `${(this.timeFraction * FULL_DASH_ARRAY).toFixed(0)} 283`;
    },

    formattedTimeLeft() {
      const timeLeft = this.timeLeft;
      const minutes = Math.floor(timeLeft / 60);
      let seconds = timeLeft % 60;

      if (seconds < 10) {
        seconds = `0${seconds}`;
      }

      return `${minutes}:${seconds}`;
    },

    timeLeft() {
      return TIME_LIMIT - this.timePassed;
    },

    timeFraction() {
      const rawTimeFraction = this.timeLeft / TIME_LIMIT;
      return rawTimeFraction - (1 / TIME_LIMIT) * (1 - rawTimeFraction);
    },

    remainingPathColor() {
      const { alert, warning, info } = COLOR_CODES;

      if (this.timeLeft <= alert.threshold) {
        return alert.color;
      } else if (this.timeLeft <= warning.threshold) {
        return warning.color;
      } else {
        return info.color;
      }
    },
  },
  watch: {
    timeLeft(newValue) {
      if (newValue === 0) {
        this.onTimesUp();
      }
    },
  },
  methods: {
    start: function () {
      this.isStarted = !this.isStarted
      if(this.isStarted === true){
        this.timerInterval = setInterval(
          () => (
            this.timePassed += 1
          ),
          1000
        )
      }else if(this.isStarted === false){
        clearInterval(this.timerInterval)
      }
    },
    onTimesUp() {
      clearInterval(this.timerInterval)
    },
  },
};
</script>

<style scoped lang="scss">
@import "./../assets/styles/first.scss";
</style>