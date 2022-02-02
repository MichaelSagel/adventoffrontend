<template>
  <!--Play on Click Component-->
  <div class="text-center py-20">
    <button
      @click="playNotification"
      class="text-2xl rounded px-8 py-2 bg-green-400 hover:bg-green-500"
    >
      Play Me
    </button>
  </div>
</template>
<script>
const notificationSound = require("@/assets/audio/key-1.mp3").default;
export default {
  name: "Home",
  data() {
    return {
      //same as notificationSound: notificationSound,
      notificationSound,
    };
  },
  methods: {
    playNotification() {
      var audio = new Audio(this.notificationSound);
      audio.play();
      console.log(audio);
    },
  },
};
</script>
<style scoped>
</style>





















<!-- <template>
  <div class="test-index">
    
  </div>
</template>

<script>
export default {

  data: function () {
    return {
    }
  },
  colorMode: "light",
  methods: {
  },
}
</script>

<style>
@import "./../assets/styles/index.scss";
</style>--> 