<template>
  <div class="third">
    <!-- <img class="piano" src="./../assets/images/third/piano.svg"/> -->
    <li v-for="item in items" :key="item.id">
    {{ item.name }}
  </li>
  </div>
</template>

<script>
export default {
  colorMode: "third",
  data: function () {
    return {
      items: [
        {
          id: 0,
          name: "French Fries with Ketchup",
          count: "1",
          price: "2.23",
          img: "./../assets/images/second/plate__french-fries.png",
        },
        {
          id: 1,
          name: "werwer",
          count: "1",
          price: "234.23",
          img: "./../assets/images/second/plate__french-fries.png",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "./../assets/styles/third.scss";
</style>