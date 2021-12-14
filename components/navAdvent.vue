<template>
  <nav class="navigation">
    <div 
      class="navigation-panel"
    >
      <NuxtLink
        to="/" 
        class="navigation-panel-element"
      >
        Home
      </NuxtLink>

      <NuxtLink
        to="/first"
        class="navigation-panel-element"
      >
        First
      </NuxtLink>
      
      <NuxtLink
        to="/second"
        class="navigation-panel-element"
      >
        Second
      </NuxtLink>

      <NuxtLink
          to="/third" 
          class="navigation-panel-element"
        >
          Third
        </NuxtLink>
    </div>
  </nav>
</template>

<style>
@import './../assets/styles/navigation.css';
</style>