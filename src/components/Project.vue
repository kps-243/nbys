<script setup>
import Button from './../components/Button.vue'
</script>
<template>
    <div class="flex flex-col gap-8">
        <div v-for="project in projects" :key="project.id" class="flex flex-col gap-10 py-3">
            <div class="flex flex-col justify-center items-center gap-5">
                <h2 class="text-2xl lg:text-4xl text-purple">{{ project.title }}</h2>
                <div class="w-full">
                  <a :href="project.link"><img :src="project.src" :alt="project.alt" class="" ></a>
                </div>
            </div>
            <div class="flex flex-col items-center lg:items-start text-center lg:text-left gap-6">
              <p class="text-lg lg:text-xl">{{ project.text }}</p>
              <Button text="View Project" :href="project.link" />
            </div>
        </div>
    </div>
</template>
<script>
export default {
  data() {
    return {
        projects: [
            {
              id: 1,
              link: "https://kps-243.github.io/Noel/",
              src: "src/assets/img/leclercnoel.webp",
              alt: "Icon - Global",
              title: "Leclerc Noel",
              text: "Give a detailed description of the service being provided here.",
            },
            {
              id: 2,
              link: "https://closethameau.fr",
              src: "src/assets/img/closethameau.png",
              alt: "Icon - Task",
              title: "Clos & Hameau",
              text: "Give a detailed description of the service being provided here.",
            },
            {
              id: 3,
              link: "https://creativehub.enzotang.fr/",
              src: "src/assets/img/creativehub.png",
              alt: "Icon - Screen",
              title: "Creative Hub",
              text: "Give a detailed description of the service being provided here.",
            }, 
        ],
    };
  },
};
</script>