<script setup lang="ts">
import Header from './components/Header.vue'
</script>

<template>
<Header/>
<router-view v-slot="{ Component }">
  <transition>
    <component :is="Component" />
  </transition>
</router-view>
</template>

<style scoped>

</style>
