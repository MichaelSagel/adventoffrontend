<template>
    <div class="fourth">
        <h1>Eyes on the Screen</h1>
        <div class="content">
            <div class="Line">
                <div class="regularButtons">`</div>
                <div class="regularButtons">1</div>
                <div class="regularButtons">2</div>
                <div class="regularButtons">3</div>
                <div class="regularButtons">4</div>
                <div class="regularButtons">5</div>
                <div class="regularButtons">6</div>
                <div class="regularButtons">7</div>
                <div class="regularButtons">8</div>
                <div class="regularButtons">9</div>
                <div class="regularButtons">0</div>
                <div class="regularButtons">-</div>
                <div class="regularButtons">=</div>
                <div class="regularButtons">DEL</div>
            </div>
            <div class="Line">
                <div class="regularButtons grayButtons">Tab</div>
                <div class="regularButtons">Q</div>
                <div class="regularButtons">E</div>
                <div class="regularButtons">R</div>
                <div class="regularButtons">T</div>
                <div class="regularButtons">Y</div>
                <div class="regularButtons">U</div>
                <div class="regularButtons">I</div>
                <div class="regularButtons">O</div>
                <div class="regularButtons">P</div>
                <div class="regularButtons">[</div>
                <div class="regularButtons">]</div>
                <div class="regularButtons">\</div>
            </div>
            <div class="Line">
                <div class="regularButtons grayButtons">CAPS</div>
                <div class="regularButtons">A</div>
                <div class="regularButtons">S</div>
                <div class="regularButtons">D</div>
                <div class="regularButtons">F</div>
                <div class="regularButtons">G</div>
                <div class="regularButtons">H</div>
                <div class="regularButtons">J</div>
                <div class="regularButtons">K</div>
                <div class="regularButtons">L</div>
                <div class="regularButtons">;</div>
                <div class="regularButtons">'</div>
                <div class="regularButtons grayButtons">ENTER</div>
            </div>
            <div class="Line">
                <div class="regularButtons grayButtons">SHIFT</div>
                <div class="regularButtons">Z</div>
                <div class="regularButtons">X</div>
                <div class="regularButtons">C</div>
                <div class="regularButtons">V</div>
                <div class="regularButtons">B</div>
                <div class="regularButtons">N</div>
                <div class="regularButtons">M</div>
                <div class="regularButtons">,</div>
                <div class="regularButtons">.</div>
                <div class="regularButtons">/</div>
                <div class="regularButtons grayButtons">SHIFT</div>
            </div>
        </div>
    </div>
</template>
<script>
export default{
    colorMode: "fourth",
  data: function () {
    return {
      keyboard: [
        {
          id: 1,
        },
        {
          id: 2,
        },
        {
          id: 3,
        },
        {
          id: 4,
        },
        {
          id: 5,
        },
        {
          id: 6,
        },
        {
          id: 7,
        },
        {
          id: 8,
        },
        {
          id: 9,
        },
        {
          id: 10,
        },
        {
          id: 11,
        },
        {
          id: 12,
        },
        {
          id: 13,
        },
        {
          id: 14,
        },
        {
          id: 15,
        },
        {
          id: 16,
        },
        {
          id: 17,
        },
        {
          id: 18,
        },
        {
          id: 19,
        },
        {
          id: 20,
        },
        {
          id: 21,
        },
        {
          id: 22,
        },
        {
          id: 23,
        },
        {
          id: 24,
        },
        {
          id: 25,
        },
        {
          id: 26,
        },
        {
          id: 27,
        },
        {
          id: 28,
        },
        {
          id: 29,
        },
        {
          id: 30,
        },
        {
          id: 31,
        },
        {
          id: 32,
        },
        {
          id: 33,
        },
        {
          id: 34,
        },
        {
          id: 35,
        },
        {
          id: 36,
        },
        {
          id: 37,
        },
        {
          id: 38,
        },
        {
          id: 39,
        },
        {
          id: 40,
        },
        {
          id: 41,
        },
        {
          id: 42,
        },
        {
          id: 43,
        },
        {
          id: 44,
        },
        {
          id: 45,
        },
        {
          id: 45,
        },
        {
          id: 46,
        },
        {
          id: 47,
        },
        {
          id: 48,
        },
        {
          id: 49,
        },
        {
          id: 50,
        },
        {
          id: 51,
        },
        {
          id: 52,
        },
      ],
    };
  },
//     methods: {
//         randomKey: function(){
//             let key = keyboard[Math.floor(Math.random()*keyboard.length)];
//             return key;
//         },
    //   beforeMount(){
    //     this.randomKey()
    //  },
//   },
}
</script>
<style scoped lang="scss">
@import "./../assets/styles/fourth.css";
</style>