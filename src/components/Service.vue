<template>
    <div v-for="service in services" :key="service.id" class="flex flex-col justify-center items-center gap-3 py-7">
        <img :src="service.src" :alt="service.alt" class="w-full h-72 object-cover" >
        <div class="flex flex-col gap-3 text-center">
            <h2 class="text-2xl text-purple">{{ service.title }}</h2>
            <p class="text-lg">{{ service.text }}</p>
        </div>
    </div>
</template>
<script>
export default {
  data() {
    return {
        services: [
            {
              id: 1,
              src: "src/assets/img/manage.jpg",
              alt: "It Support",
              title: "Manage It Services",
              text: "Give a detailed description of the service being provided here.",
            },
            {
              id: 2,
              src: "src/assets/img/it-security.jpg",
              alt: "It Security",
              title: "It Security",
              text: "Give a detailed description of the service being provided here.",
            },
            {
              id: 3,
              src: "src/assets/img/it-consulting.jpg",
              alt: "It Consulting",
              title: "It Consulting",
              text: "Give a detailed description of the service being provided here.",
            },
            
        ],
    };
  },
};
</script>