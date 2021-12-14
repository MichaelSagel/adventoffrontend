<template>
  <div 
    class="first"
  >
    <div 
      class="timer"
  
    >
    </div>
    <div 
      class="start-or-stop"
      @click="isStarted = !isStarted"
    >
     {{ isStarted ? 'S T O P' : 'S T A R T' }}
    </div>


  <div
    class="circle"
  >
  </div>

  <div 
    class="gear"
  >
      <img src="./../assets/images/gear.svg">
  </div>
    
  </div>
</template>

<script>
  export default {
    colorMode: 'first',
    data: function () {
      return {
        isHidden: false,
        isStarted: false,
      }
    },
    methods: {
      refresh: function() {
        this.isHidden = !this.isHidden
        this.$nuxt.refresh();
      },
    },
  }
</script>

<style>
@import './../assets/styles/first.css';
</style>