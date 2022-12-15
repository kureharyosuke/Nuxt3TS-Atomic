<template>
  <select :id="id" :name="name">
    <option v-for="{ id, value } in select" :key="id" :value="value">
      {{ value }}
    </option>
  </select>
</template>

<script setup lang="ts">
type Props = {
  id: string;
  name: string;
  select: { id: number | string; value: string }[];
};
defineProps<Props>();
</script>

<style scoped></style>
