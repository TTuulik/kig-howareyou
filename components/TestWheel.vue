<script setup>
const { size = 400 } = defineProps(["size"]);
</script>

<template>
  <svg :width="size" :height="size" class="block">
    <g :transform="translate(size / 2, size / 2)"><slot /></g>
  </svg>
</template>
