<template>
  <div class="fourth">
    <h1>Eyes on the Screen</h1>
    <div class="content">
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
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 2,
              value: 1,
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 3,
              value: 2,
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 4,
              value: 3,
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 5,
              value: 4,
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 6,
              value: 5,
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 7,
              value: 6,
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 8,
              value: 7,
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 9,
              value: 8,
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 10,
              value: 9,
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 11,
              value: 0,
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 12,
              value: "-",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 13,
              value: "=",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 14,
              value: "DEL",
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
              value: "E",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 18,
              value: "R",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 19,
              value: "T",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 20,
              value: "Y",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 21,
              value: "U",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 22,
              value: "I",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 23,
              value: "O",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 24,
              value: "P",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 25,
              value: "[",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 26,
              value: "]",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 27,
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
              id: 28,
              value: "CAPS",
              color: "#868888",
              background: "#FFFFFF",
            },
            {
              id: 29,
              value: "A",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 30,
              value: "S",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 31,
              value: "D",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 32,
              value: "F",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 33,
              value: "G",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 34,
              value: "H",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 35,
              value: "j",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 36,
              value: "K",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 37,
              value: "L",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 38,
              value: ";",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 39,
              value: "'",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 40,
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
              id: 41,
              value: "SHIFT",
              color: "#868888",
              background: "#FFFFFF",
            },
            {
              id: 42,
              value: "Z",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 43,
              value: "X",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 44,
              value: "C",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 45,
              value: "V",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 45,
              value: "B",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 46,
              value: "N",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 47,
              value: "M",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 48,
              value: ",",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 49,
              value: ".",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 50,
              value: "/",
              color: "#60C1B6",
              background: "#FFFFFF",
            },
            {
              id: 51,
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
      let max = 51;
      let randomnumber = Math.floor(Math.random() * (max - min)) + min;
      console.log(randomnumber);
      this.selectedId = randomnumber;
      let pressedButton = document.addEventListener('keydown');
      if (pressedButton === element.value){

      }
    },
  },
};
</script>
<style scoped lang="scss">
@import "./../assets/styles/fourth.css";
</style>