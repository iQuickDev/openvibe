<script setup lang="ts">
import { ref } from 'vue';
import LiquidGauge from '../components/LiquidGauge.vue';

const percentage = ref(100);

setInterval(() => {
    percentage.value = percentage.value - 1;
}, 100);

</script>

<template>
    <div class="flex flex-row justify-center items-center h-100">
        <LiquidGauge :percentage="percentage" />
    </div>

</template>

<style scoped></style>
