<script setup>
defineProps({
  text: {
    type: String,
    required: true
  }
})
</script>
<template>
  <div>
    <a :href="link">
      <button class="text-purple hover:text-black hover:bg-white ease-in-out transition-all duration-100 px-10 py-3 rounded-full border border-purple lg:text-lg lg:px-16">
        {{ text }}
      </button>
    </a>
  </div>
</template>
<script>

</script>