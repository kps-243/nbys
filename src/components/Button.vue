<script setup>
defineProps({
  text: {
    type: String,
    required: true
  }
})
</script>
<template>
    <a :href="link">
      <button class="text-purple px-10 py-3 rounded-full border border-purple">
        {{ text }}
    </button>
    </a>
</template>
<script>

</script>