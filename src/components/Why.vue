<template>
    <div class="w-4/6 flex flex-col items-center justify-center gap-8">
        <div v-for="why in whys" :key="why.id" class="flex flex-col justify-center items-center gap-3 py-24 px-5 border border-purple rounded-[70px] ">
            <div class="flex flex-col gap-5 text-center">
                <h2 class="text-2xl text-purple">{{ why.title }}</h2>
                <img :src="why.src" :alt="why.alt" class="w-full h-16" >
                <p class="text-lg">{{ why.text }}</p>
            </div>
        </div>
    </div>
</template>
<script>
export default {
  data() {
    return {
        whys: [
            {
              id: 1,
              src: "src/assets/img/global.svg",
              alt: "Icon - Global",
              title: "We are global.",
              text: "Give a detailed description of the service being provided here.",
            },
            {
              id: 2,
              src: "src/assets/img/task.svg",
              alt: "Icon - Task",
              title: "We are task oriented.",
              text: "Give a detailed description of the service being provided here.",
            },
            {
              id: 3,
              src: "src/assets/img/screen.svg",
              alt: "Icon - Screen",
              title: "We are digital.",
              text: "Give a detailed description of the service being provided here.",
            },
            
        ],
    };
  },
};
</script>