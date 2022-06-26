<script setup>
defineProps({
  title: {
    type: String,
    required: true,
  },
});
</script>
<template>
  <h1>Home - {{ title }}</h1>
</template>
