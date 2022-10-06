<script setup>
const { options } = defineProps(["options"]);
defineEmits(["select"]);
</script>

<template>
  <div class="grid grid-cols-2 gap-4 p-8">
    <div
      v-for="(option, i) in options"
      class="aspect-square bg-red-500 grid place-items-center text-center text-8xl p-6"
      :class="[
        [
          'rounded-tl-[550px]',
          'rounded-tr-[550px]',
          'rounded-bl-[550px]',
          'rounded-br-[550px]',
        ][i % 4],
      ]"
      :style="{ background: option.fill }"
      @click="$emit('select', option)"
    >
      <div class="opacity-80">{{ option.title }}</div>
    </div>
  </div>
</template>
