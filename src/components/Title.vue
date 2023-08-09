<script setup>
defineProps({
  title: {
    type: String,
    required: true
  }
})
</script>
<template>
    <h1 class="text-purple text-center text-3xl lg:text-6xl">{{ title }}</h1>
</template>