<template>
  <div class="test-index">
    <button
      class="btn-primary"
      @click="refresh"
    >
      <template v-if="isHidden">Click to Show</template>
      <template v-else>Click to Hide</template>
    </button>

    <button 
      class="test"
      @click="isStarted = !isStarted"
    >
     {{ isStarted ? 'Stop' : 'Start' }}
    </button>
  </div>
</template>

<script>
export default {

  data: function () {
    return {
      isHidden: false,
      isStarted: false,
    }
  },
  colorMode: "light",
  methods: {
    refresh: function() {
      this.isHidden = !this.isHidden
      this.$nuxt.refresh();
    },
  },
}
</script>

<style>
@import "./../assets/styles/index.scss";
</style>