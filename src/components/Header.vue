<script setup>
</script>
<template>
    <div class="pt-6">
      <div class="flex justify-between items-center">
        <img alt="Nbys logo" class="z-20 w-14 h-auto" src="./../assets/img/logo.svg" />
        <div class="lg:hidden">
            <div class="">
                <img  v-if="!menuOpen" @click="toggleMenu" src="./../assets/img/burger.svg" alt="NbyS - icon Burger">
                <img  v-if="menuOpen" @click="toggleMenu" src="./../assets/img/close.svg" alt="NbyS - icon Close">
            </div>
        </div>
      </div>
      <div v-if="menuOpen" class="lg:hidden z-10 h-screen flex items-center justify-center">
          <ul class="flex flex-col gap-10">
            <li v-for="(menuItem, index) in menuItems" :key="index" class="text-2xl hover:text-white">
              {{ menuItem }}
            </li>
          </ul>
      </div>   
    </div>
</template>
<script>
export default {
  data() {
    return {
      menuOpen: false,
      menuItems: ["Home", "About", "Contact"],
    };
  },
  methods: {
    toggleMenu() {
      this.menuOpen = !this.menuOpen;
    },
  },
};
</script>