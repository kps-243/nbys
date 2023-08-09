<script setup>
</script>
<template>
  <header>
    <div class="pt-6">
      <div class="container flex justify-between items-center">
        <img alt="Nbys logo" class="z-20 w-14 h-auto" src="./../assets/img/logo.svg" />
        <div class="lg:hidden">
          <img  v-if="!menuOpen" @click="toggleMenu" src="./../assets/img/burger.svg" alt="NbyS - icon Burger">
          <img  v-if="menuOpen" @click="toggleMenu" src="./../assets/img/close.svg" alt="NbyS - icon Close">
        </div>
      </div>
      <div v-if="menuOpen" class="lg:hidden z-10 h-screen w-full flex pt-16">
          <ul class="flex flex-col text-center w-full">
            <li v-for="(menuItem, index) in menuItems" :key="index" class="w-full py-6 text-2xl transition-all duration-200 hover:text-black hover:bg-white">
              {{ menuItem }}
            </li>
          </ul>
      </div>   
    </div>
  </header>
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