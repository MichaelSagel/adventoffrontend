<template>
  <div class="fourth">
    <h1>Eyes on the Screen</h1>
    <div 
      class="content"
    >
      <div 
        class="line"
        v-for="item in keyboard"
        :key="item.id"
      >
        <div
          class="regular-buttons"
          v-for="element in item.line"
          :key="element.id"
          :class="{
            play:selectedId === element.id
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
  },
  data: function () {
    return {
      selectedId:0,
      keyboard: [
        {
          id:0,
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
          id:1,
          line: [
            {
              id: 15,
              value: "Tab",
              color: "#868888",
              background: "#FFFFFF",
            },
            {
              id: 16,
              value: "Q",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 17,
              value: "W",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 18,
              value: "E",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 19,
              value: "R",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 20,
              value: "T",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 21,
              value: "Y",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 22,
              value: "U",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 23,
              value: "I",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 24,
              value: "O",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 25,
              value: "P",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 26,
              value: "[",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 27,
              value: "]",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 28,
              value: "\\",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
          ],
        },
        {
          id:2,
          line: [
            {
              id: 29,
              value: "CAPS",
              color: "#868888",
              background: "#FFFFFF",
            },
            {
              id: 30,
              value: "A",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 31,
              value: "S",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 32,
              value: "D",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 33,
              value: "F",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 34,
              value: "G",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 35,
              value: "H",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 36,
              value: "j",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 37,
              value: "K",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 38,
              value: "L",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 39,
              value: ";",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 40,
              value: "'",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 41,
              value: "ENTER",
              color: "#868888",
              background: "#FFFFFF",
            },
          ],
        },
        {
          id:3,
          line: [
            {
              id: 42,
              value: "SHIFT",
              color: "#868888",
              background: "#FFFFFF",
            },
            {
              id: 43,
              value: "Z",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 44,
              value: "X",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 45,
              value: "C",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 46,
              value: "V",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 47,
              value: "B",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 48,
              value: "N",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 49,
              value: "M",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 50,
              value: ",",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 51,
              value: ".",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 52,
              value: "/",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 53,
              value: "SHIFT",
              color: "#868888",
              background: "#FFFFFF",
            },
          ],
        },
      ],
    };
  },
  methods: {
    randomKey: function () {
      let min = 1;
      let max = 14; //53
      let randomnumber = Math.floor(Math.random() * (max - min)) + min;
      this.selectedId = randomnumber;

      document.addEventListener("keydown", (keyDownEvent) => {
        // мы прозодимся по всем кнопкам в наших массивах 
        this.keyboard.forEach((item) => {
          // item это не кнопка!
          console.log(item)
          // мы смотрим что ID перед которыми мы итэрируемся сейчас это текушая выбраная кнопка
          // и проверяем что код нажатой кнопки совподает с кодом кнопки текущей итэрации
          if (item.id === selectedId && item.keyCode === keyDownEvent.code) {
            this.randomKey();
          }
        });
      })
    },
  },
};
</script>
<style scoped lang="scss">
@import "./../assets/styles/fourth.css";
</style>