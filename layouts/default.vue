<template>
    <div class="global">
        <navAdvent/>
        <Nuxt />
    </div>
</template>

<script>
  import navAdvent from './../components/navAdvent.vue';

  export default ({
    components: {
      navAdvent,
    },
  });
</script>

<style>
@import './../assets/styles/global.css';
</style>