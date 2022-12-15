<template>
  <input :id="id" :name="name" :type="type" />
</template>

<script setup lang="ts">
type Props = {
  id?: string;
  name?: string;
  type: "text" | "email" | "password" | "tel";
};
defineProps<Props>();
</script>

<style scoped></style>
