<script setup>
defineProps({
  title: {
    type: String,
    required: true,
  },
});
</script>

<template>
  <div class="flex items-center gap-5">
    <input type="checkbox" class="border" />
    <p>Awikwo</p>
  </div>
</template>
