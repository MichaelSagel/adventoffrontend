<template>
  <div class="fourth">
    <h1>Eyes on the Screen</h1>
    <div class="content">
      <div class="line" v-for="item in keyboard" :key="item.id">
        <div
          class="regular-buttons"
          v-for="element in item.line"
          :key="element.id"
          :class="{
            play: selectedId === element.id,
          }"
          :style="{
            '--key-color': element.color,
            '--key-background-color': element.background,
          }"
        >
          {{ element.value }}
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
    document.addEventListener("keydown", this.hz);
  },
  destroyed() {
    document.removeEventListener("keydown", this.hz);
  },
  data: function () {
    return {
      selectedId: 0,
      keyboard: [
        {
          id: 0,
          line: [
            {
              id: 1,
              value: "`",
              keyCode: "Equal",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 2,
              value: 1,
              keyCode: "Digit1",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 3,
              value: 2,
              keyCode: "Digit2",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 4,
              value: 3,
              keyCode: "Digit3",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 5,
              value: 4,
              keyCode: "Digit4",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 6,
              value: 5,
              keyCode: "Digit5",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 7,
              value: 6,
              keyCode: "Digit6",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 8,
              value: 7,
              keyCode: "Digit7",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 9,
              value: 8,
              keyCode: "Digit8",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 10,
              value: 9,
              keyCode: "Digit9",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 11,
              value: 0,
              keyCode: "Digit0",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 12,
              value: "-",
              keyCode: "Slash",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 13,
              value: "=",
              keyCode: "Equal",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 14,
              value: "DEL",
              keyCode: "Backspace",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
          ],
        },
        {
          id: 1,
          line: [
            {
              id: 15,
              value: "Tab",
              keyCode: "Tab",
              color: "#868888",
              background: "#FFFFFF",
            },
            {
              id: 16,
              value: "Q",
              keyCode: "KeyQ",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 17,
              value: "W",
              keyCode: "KeyW",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 18,
              value: "E",
              keyCode: "KeyE",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 19,
              value: "R",
              keyCode: "KeyR",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 20,
              value: "T",
              keyCode: "KeyT",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 21,
              value: "Y",
              keyCode: "KeyY",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 22,
              value: "U",
              keyCode: "KeyU",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 23,
              value: "I",
              keyCode: "KeyI",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 24,
              value: "O",
              keyCode: "KeyO",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 25,
              value: "P",
              keyCode: "KeyP",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 26,
              value: "[",
              keyCode: "Digit8",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 27,
              value: "]",
              keyCode: "Digit9",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 28,
              value: "\\",
              keyCode: "Minus",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
          ],
        },
        {
          id: 2,
          line: [
            {
              id: 29,
              value: "CAPS",
              keyCode: "CapsLock",
              color: "#868888",
              background: "#FFFFFF",
            },
            {
              id: 30,
              value: "A",
              keyCode: "KeyA",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 31,
              value: "S",
              keyCode: "KeyS",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 32,
              value: "D",
              keyCode: "KeyD",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 33,
              value: "F",
              keyCode: "KeyF",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 34,
              value: "G",
              keyCode: "KeyG",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 35,
              value: "H",
              keyCode: "KeyH",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 36,
              value: "j",
              keyCode: "KeyJ",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 37,
              value: "K",
              keyCode: "KeyK",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 38,
              value: "L",
              keyCode: "KeyL",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 39,
              value: ";",
              keyCode: "Comma",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 40,
              value: "'",
              keyCode: "Equal",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 41,
              value: "ENTER",
              keyCode: "Enter",
              color: "#868888",
              background: "#FFFFFF",
            },
          ],
        },
        {
          id: 3,
          line: [
            {
              id: 42,
              value: "SHIFT",
              keyCode: "ShiftLeft",
              color: "#868888",
              background: "#FFFFFF",
            },
            {
              id: 43,
              value: "Z",
              keyCode: "KeyZ",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 44,
              value: "X",
              keyCode: "KeyX",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 45,
              value: "C",
              keyCode: "KeyC",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 46,
              value: "V",
              keyCode: "KeyV",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 47,
              value: "B",
              keyCode: "KeyB",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 48,
              value: "N",
              keyCode: "KeyN",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 49,
              value: "M",
              keyCode: "KeyM",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 50,
              value: ",",
              keyCode: "Comma",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 51,
              value: ".",
              keyCode: "Period",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 52,
              value: "/",
              keyCode: "Digit7",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 53,
              value: "SHIFT",
              keyCode: "ShiftRight",
              color: "#868888",
              background: "#FFFFFF",
            },
          ],
        },
      ],
    };
  },
  methods: {
    hz: function (keyDownEvent)  {
      console.log("item");
      this.keyboard.forEach((item) => {
        item.line.forEach((items) => {
          if (
            items.id === this.selectedId &&
            items.keyCode === keyDownEvent.code
          ) {
            this.randomKey();
          }
        });
      });
    },
    randomKey: function () {
      let min = 1;
      let max = 53; //53
      let randomnumber = Math.floor(Math.random() * (max - min)) + min;
      this.selectedId = randomnumber;
      
    },
  },
};
</script>
<style scoped lang="scss">
@import "./../assets/styles/fourth.css";
</style>