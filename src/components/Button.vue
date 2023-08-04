<script setup>
defineProps({
  text: {
    type: String,
    required: true
  }
})
</script>
<template>
    <button class="text-purple px-10 py-3 rounded-full border border-purple">
        {{ text }}
    </button>
</template>
<script>

</script>