<template>
    <div class="flex flex-col min-h-screen">
      <BaseSiteHeader :key="$route.fullPath"></BaseSiteHeader>
      <slot/>
      <div class="flex-grow justify-center"></div>
      <BasePageFooter1 />
    </div>
  </template>
  
  <script setup lang="ts">
  
  </script>
  