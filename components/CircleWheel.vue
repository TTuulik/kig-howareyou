<script setup>
const { options = [] } = defineProps(["options"]);
defineEmits(["select"]);

const items = options.map((option, i) => {
  const point = polar(i * (180 / (options.length - 1)), 270);
  return { ...option, point };
});
</script>
<template>
  <div class="relative">
    <button
      v-for="(item, i) in items"
      @click="$emit('select', item)"
      class="w-24 text-sm rounded-full h-24 absolute bg-black text-white grid place-items-center text-center -translate-x-5 -translate-y-5"
      :style="{
        left: item.point.x / 1.3 + 'px',
        top: i * 100 + 'px',
        background: item.fill,
      }"
    >
      {{ item.title }}
    </button>
  </div>
</template>
