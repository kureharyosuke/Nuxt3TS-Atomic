<template>
  <ul>
    <li v-for="{ id, value } in list" :key="id">{{ value }}</li>
  </ul>
</template>

<script setup lang="ts">
type Props = {
  list: { id: number | string; value: string }[];
};
defineProps<Props>();
</script>

<style scoped></style>
