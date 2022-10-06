<script setup>
import { interpolateSinebow } from "d3";
const { options } = defineProps(["options"]);
defineEmits(["select"]);
</script>

<template>
  <div class="grid grid-cols-2 gap-1 p-4">
    <div
      v-for="(option, i) in options"
      class="aspect-square bg-red-500 grid place-items-center text-center p-6"
      :class="[
        [
          'rounded-tl-[50px]',
          'rounded-tr-[50px]',
          'rounded-bl-[50px]',
          'rounded-br-[50px]',
        ][i % 4],
      ]"
      :style="{ background: option.fill }"
      @click="$emit('select', option)"
    >
      <div class="opacity-80">{{ option.title }}</div>
    </div>
  </div>
</template>
