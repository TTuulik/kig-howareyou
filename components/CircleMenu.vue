<script setup>
import { interpolateSinebow } from "d3";
const { options } = defineProps(["options"]);
defineEmits(["select"]);
</script>

<template>
  <div class="grid grid-cols-2 gap-4 p-8">
    <div
      v-for="(option, i) in options"
      class="aspect-square bg-red-500 grid place-items-center text-center text-4xl p-6"
      :class="[
        [
          'rounded-tl-[150px]',
          'rounded-tr-[150px]',
          'rounded-bl-[150px]',
          'rounded-br-[150px]',
        ][i % 4],
      ]"
      :style="{ background: option.fill }"
      @click="$emit('select', option)"
    >
      <div class="opacity-80">{{ option.title }}</div>
    </div>
  </div>
</template>
