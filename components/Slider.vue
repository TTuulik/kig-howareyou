<script setup lang="ts">
type Props = {
  modelValue?: number;
};

type Emits = {
  (e: "update:modelValue", value: number): void;
};

const { modelValue = "" } = defineProps<Props>();

const emit = defineEmits<Emits>();

const inputValue = computed({
  get: () => modelValue,
  set: (value) => {
    emit("update:modelValue", value);
  },
});
</script>

<template>
  <input
    type="range"
    v-model.number="inputValue"
    class="accent-gray-500 block h-px cursor-pointer appearance-auto bg-gray-500 w-3/4 md:w-64"
  />
</template>
