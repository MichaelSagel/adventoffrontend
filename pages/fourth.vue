<template>
  <div class="fourth">
    <h1>Eyes on the Screen</h1>
    <div class="content">
      <div class="line">
        <div
          class="regular-buttons"
          v-for="item in keyboard_first_line"
          :key="item.id"
          :style="{
            '--key-color': item.color,
            '--key-background-color': item.background,
          }"
        >
          {{ item.meaning }}
        </div>
      </div>
      <div class="line">
        <div
          class="regular-buttons"
          v-for="item in keyboard_second_line"
          :key="item.id"
          :style="{
            '--key-color': item.color,
            '--key-background-color': item.background,
          }"
        >
          {{ item.meaning }}
        </div>
      </div>
      <div class="line">
        <div
          class="regular-buttons"
          v-for="item in keyboard_third_line"
          :key="item.id"
          :style="{
            '--key-color': item.color,
            '--key-background-color': item.background,
          }"
        >
          {{ item.meaning }}
        </div>
      </div>
      <div class="line">
        <div
          class="regular-buttons"
          v-for="item in keyboard_fourth_line"
          :key="item.id"
          :style="{
            '--key-color': item.color,
            '--key-background-color': item.background,
          }"
        >
          {{ item.meaning }}
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  colorMode: "fourth",
  beforeMount() {
    this.randomKey();
  },
  data: function () {
    return {
      keyboard_first_line: [
        {
          id: 1,
          meaning: "`",
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 2,
          meaning: 1,
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 3,
          meaning: 2,
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 4,
          meaning: 3,
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 5,
          meaning: 4,
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 6,
          meaning: 5,
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 7,
          meaning: 6,
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 8,
          meaning: 7,
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 9,
          meaning: 8,
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 10,
          meaning: 9,
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 11,
          meaning: 0,
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 12,
          meaning: "-",
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 13,
          meaning: "=",
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 14,
          meaning: "DEL",
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
      ],
      keyboard_second_line: [
        {
          id: 15,
          meaning: "Tab",
          color: "#868888",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 16,
          meaning: "Q",
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 17,
          meaning: "E",
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 18,
          meaning: "R",
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 19,
          meaning: "T",
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 20,
          meaning: "Y",
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 21,
          meaning: "U",
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 22,
          meaning: "I",
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 23,
          meaning: "O",
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 24,
          meaning: "P",
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 25,
          meaning: "[",
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 26,
          meaning: "]",
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 27,
          meaning: "\\",
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
      ],
      keyboard_third_line: [
        {
          id: 28,
          meaning: "CAPS",
          color: "#868888",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 29,
          meaning: "A",
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 30,
          meaning: "S",
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 31,
          meaning: "D",
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 32,
          meaning: "F",
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 33,
          meaning: "G",
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 34,
          meaning: "H",
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 35,
          meaning: "j",
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 36,
          meaning: "K",
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 37,
          meaning: "L",
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 38,
          meaning: ";",
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 39,
          meaning: "'",
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 40,
          meaning: "ENTER",
          color: "#868888",
          background: "#FFFFFF",
          chosen: false,
        },
      ],
      keyboard_fourth_line: [
        {
          id: 41,
          meaning: "SHIFT",
          color: "#868888",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 42,
          meaning: "Z",
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 43,
          meaning: "X",
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 44,
          meaning: "C",
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 45,
          meaning: "V",
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 45,
          meaning: "B",
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 46,
          meaning: "N",
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 47,
          meaning: "M",
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 48,
          meaning: ",",
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 49,
          meaning: ".",
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 50,
          meaning: "/",
          color: "#60C1B6",
          background: "#FFFFFF",
          chosen: false,
        },
        {
          id: 51,
          meaning: "SHIFT",
          color: "#868888",
          background: "#FFFFFF",
          chosen: false,
        },
      ],
    };
  },
  methods: {
    randomKey: function () {
      let min = 1;
      let max = 14;
      let randomnumber = Math.floor(Math.random() * (max - min)) + min;
      console.log(randomnumber);
      const elem = this.keyboard_first_line.find(function (element) {
        return element.id === randomnumber;
      });
      elem.classList.add("test");
    },
  },
};
</script>
<style scoped lang="scss">
@import "./../assets/styles/fourth.css";
</style>