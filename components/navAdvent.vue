<template>
  <nav class="navigation">
    <div 
      class="navigationPanel"
    >
      <NuxtLink
        to="/" 
        class="navigationPanelElement"
      >
        Home
      </NuxtLink>

      <NuxtLink
        to="/first"
        class="navigationPanelElement"
      >
        First
      </NuxtLink>
      
      <NuxtLink
        to="/second"
        class="navigationPanelElement"
      >
        Second
      </NuxtLink>

      <NuxtLink
          to="/third" 
          class="navigationPanelElement"
        >
          Third
        </NuxtLink>

        <NuxtLink
          to="/fourth" 
          class="navigationPanelElement"
        >
          Fourth
        </NuxtLink>
    </div>
  </nav>
</template>

<style>
@import './../assets/styles/navigation.css';
</style>