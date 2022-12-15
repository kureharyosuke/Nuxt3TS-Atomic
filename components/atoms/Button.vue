<template>
  <button :type="type" :disabled="disabled">
    {{ value }}
  </button>
</template>

<script setup lang="ts">
type Props = {
  value: string;
  type: "button" | "reset" | "submit";
  disabled: boolean;
  onClick: (payload: MouseEvent) => void | undefined;
};
defineProps<Props>();
</script>

<style scoped></style>
