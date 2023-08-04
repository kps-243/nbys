<script setup>
defineProps({
  title: {
    type: String,
    required: true
  }
})
</script>
<template>
    <h1 class="text-purple text-3xl">{{ title }}</h1>
</template>