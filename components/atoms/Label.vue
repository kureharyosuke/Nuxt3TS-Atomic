<template>
  <label :html-for="htmlFor">{{ value }}</label>
</template>

<script setup lang="ts">
type Props = {
  htmlFor?: string;
  value: string;
};
defineProps<Props>();
</script>

<style scoped></style>
