<template>
    <div class="fourth">
        <h1>Eyes on the Screen</h1>
        <div class="content">
            <div class="Line">
                <div class="regularButtons">{{keyboard[0].meaning}}</div>
                <div class="regularButtons">{{keyboard[1].meaning}}</div>
                <div class="regularButtons">{{keyboard[2].meaning}}</div>
                <div class="regularButtons">{{keyboard[3].meaning}}</div>
                <div class="regularButtons">{{keyboard[4].meaning}}</div>
                <div class="regularButtons">{{keyboard[5].meaning}}</div>
                <div class="regularButtons">{{keyboard[6].meaning}}</div>
                <div class="regularButtons">{{keyboard[7].meaning}}</div>
                <div class="regularButtons">{{keyboard[8].meaning}}</div>
                <div class="regularButtons">{{keyboard[9].meaning}}</div>
                <div class="regularButtons">{{keyboard[10].meaning}}</div>
                <div class="regularButtons">{{keyboard[11].meaning}}</div>
                <div class="regularButtons">{{keyboard[12].meaning}}</div>
                <div class="regularButtons">{{keyboard[13].meaning}}</div>
            </div>
            <div class="Line">
                <div class="regularButtons grayButtons">{{keyboard[14].meaning}}</div>
                <div class="regularButtons">{{keyboard[15].meaning}}</div>
                <div class="regularButtons">{{keyboard[16].meaning}}</div>
                <div class="regularButtons">{{keyboard[17].meaning}}</div>
                <div class="regularButtons">{{keyboard[18].meaning}}</div>
                <div class="regularButtons">{{keyboard[19].meaning}}</div>
                <div class="regularButtons">{{keyboard[20].meaning}}</div>
                <div class="regularButtons">{{keyboard[21].meaning}}</div>
                <div class="regularButtons">{{keyboard[22].meaning}}</div>
                <div class="regularButtons">{{keyboard[23].meaning}}</div>
                <div class="regularButtons">{{keyboard[24].meaning}}</div>
                <div class="regularButtons">{{keyboard[25].meaning}}</div>
                <div class="regularButtons">{{keyboard[26].meaning}}</div>
            </div>
            <div class="Line">
                <div class="regularButtons grayButtons">{{keyboard[27].meaning}}</div>
                <div class="regularButtons">{{keyboard[28].meaning}}</div>
                <div class="regularButtons">{{keyboard[29].meaning}}</div>
                <div class="regularButtons">{{keyboard[30].meaning}}</div>
                <div class="regularButtons">{{keyboard[31].meaning}}</div>
                <div class="regularButtons">{{keyboard[32].meaning}}</div>
                <div class="regularButtons">{{keyboard[33].meaning}}</div>
                <div class="regularButtons">{{keyboard[34].meaning}}</div>
                <div class="regularButtons">{{keyboard[35].meaning}}</div>
                <div class="regularButtons">{{keyboard[36].meaning}}</div>
                <div class="regularButtons">{{keyboard[37].meaning}}</div>
                <div class="regularButtons">{{keyboard[38].meaning}}</div>
                <div class="regularButtons grayButtons">{{keyboard[39].meaning}}</div>
            </div>
            <div class="Line">
                <div class="regularButtons grayButtons">{{keyboard[40].meaning}}</div>
                <div class="regularButtons">{{keyboard[41].meaning}}</div>
                <div class="regularButtons">{{keyboard[42].meaning}}</div>
                <div class="regularButtons">{{keyboard[43].meaning}}</div>
                <div class="regularButtons">{{keyboard[44].meaning}}</div>
                <div class="regularButtons">{{keyboard[45].meaning}}</div>
                <div class="regularButtons">{{keyboard[46].meaning}}</div>
                <div class="regularButtons">{{keyboard[47].meaning}}</div>
                <div class="regularButtons">{{keyboard[48].meaning}}</div>
                <div class="regularButtons">{{keyboard[49].meaning}}</div>
                <div class="regularButtons">{{keyboard[50].meaning}}</div>
                <div class="regularButtons grayButtons">{{keyboard[51].meaning}}</div>
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
          meaning:"`",
          chosen: false,
        },
        {
          id: 2,
          meaning:1,
          chosen: false,
        },
        {
          id: 3,
          meaning:2,
          chosen: false,
        },
        {
          id: 4,
          meaning:3,
          chosen: false,
        },
        {
          id: 5,
          meaning:4,
          chosen: false,
        },
        {
          id: 6,
          meaning:5,
          chosen: false,
        },
        {
          id: 7,
          meaning:6,
          chosen: false,
        },
        {
          id: 8,
          meaning:7,
          chosen: false,
        },
        {
          id: 9,
          meaning:8,
          chosen: false,
        },
        {
          id: 10,
          meaning:9,
          chosen: false,
        },
        {
          id: 11,
          meaning:0,
          chosen: false,
        },
        {
          id: 12,
          meaning:"-",
          chosen: false,
        },
        {
          id: 13,
          meaning:"=",
          chosen: false,
        },
        {
          id: 14,
          meaning:"DEL",
          chosen: false,
        },
        {
          id: 15,
          meaning:"Tab",
          chosen: false,
        },
        {
          id: 16,
          meaning:"Q",
          chosen: false,
        },
        {
          id: 17,
          meaning:"E",
          chosen: false,
        },
        {
          id: 18,
          meaning:"R",
          chosen: false,
        },
        {
          id: 19,
          meaning:"T",
          chosen: false,
        },
        {
          id: 20,
          meaning:"Y",
          chosen: false,
        },
        {
          id: 21,
          meaning:"U",
          chosen: false,
        },
        {
          id: 22,
          meaning:"I",
          chosen: false,
        },
        {
          id: 23,
          meaning:"O",
          chosen: false,
        },
        {
          id: 24,
          meaning:"P",
          chosen: false,
        },
        {
          id: 25,
          meaning:"[",
          chosen: false,
        },
        {
          id: 26,
          meaning:"]",
          chosen: false,
        },
        {
          id: 27,
          meaning:"\\",
          chosen: false,
        },
        {
          id: 28,
          meaning:"CAPS",
          chosen: false,
        },
        {
          id: 29,
          meaning:"A",
          chosen: false,
        },
        {
          id: 30,
          meaning:"S",
          chosen: false,
        },
        {
          id: 31,
          meaning:"D",
          chosen: false,
        },
        {
          id: 32,
          meaning:"F",
          chosen: false,
        },
        {
          id: 33,
          meaning:"G",
          chosen: false,
        },
        {
          id: 34,
          meaning:"H",
          chosen: false,
        },
        {
          id: 35,
          meaning:"j",
          chosen: false,
        },
        {
          id: 36,
          meaning:"K",
          chosen: false,
        },
        {
          id: 37,
          meaning:"L",
          chosen: false,
        },
        {
          id: 38,
          meaning:";",
          chosen: false,
        },
        {
          id: 39,
          meaning:"'",
          chosen: false,
        },
        {
          id: 40,
          meaning:"ENTER",
          chosen: false,
        },
        {
          id: 41,
          meaning:"SHIFT",
          chosen: false,
        },
        {
          id: 42,
          meaning:"Z",
          chosen: false,
        },
        {
          id: 43,
          meaning:"X",
          chosen: false,
        },
        {
          id: 44,
          meaning:"C",
          chosen: false,
        },
        {
          id: 45,
          meaning:"V",
          chosen: false,
        },
        {
          id: 45,
          meaning:"B",
          chosen: false,
        },
        {
          id: 46,
          meaning:"N",
          chosen: false,
        },
        {
          id: 47,
          meaning:"M",
          chosen: false,
        },
        {
          id: 48,
          meaning:",",
          chosen: false,
        },
        {
          id: 49,
          meaning:".",
          chosen: false,
        },
        {
          id: 50,
          meaning:"/",
          chosen: false,
        },
        {
          id: 51,
          meaning:"SHIFT",
          chosen: false,
        },
      ],
    };
  },
  methods:{
   
  },
    methods: {
      beforeMount(){
        this.randomKey()
        console.log(aaaaaaa);
      },
      randomKey: function(){
        let key = keyboard[Math.floor(Math.random()*keyboard.length)];
        console.log(key);
        return key;
      },
   },
}
</script>
<style scoped lang="scss">
@import "./../assets/styles/fourth.css";
</style>