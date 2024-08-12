<template>
  <header
    class="fixed top-0 left-0 z-30 w-full bg-white shadow-shadow py-[9px]"
  >
    <div
      class="flex items-center justify-between max-w-screen-sm px-5 mx-auto md:max-w-screen-md lg:max-w-screen-lg xl:max-w-screen-xl"
    >
      <router-link
        class="flex items-center gap-2.5 font-compact md:text-xl text-lg leading-6 text-txt font-normal"
        to="/"
        ><div class="md:w-[50px] md:h-[50px] w-8 h-8"><HeaderLogo /></div>
        Тестирование</router-link
      >
      <div class="flex items-center gap-4">
        <router-link
          class="md:flex items-center p-2.5 text-17 leading-6 font-medium font-wide text-txt hidden"
          to="/balance"
          ><span class="px-2 py-1">Поддержка</span></router-link
        >
        <router-link
          class="flex items-center md:p-2.5 p-1.5 md:text-xs text-[10px] font-bold tracking-wider uppercase font-wide text-white rounded-2xl bg-brand"
          to="/purchases"
          ><span class="px-2 py-1">Войти</span></router-link
        >
      </div>
    </div>
  </header>
</template>

<script setup>
import HeaderLogo from "./icons/HeaderLogo.vue";
import Wallet from "./icons/Wallet.vue";
import CartLogo from "./icons/CartLogo.vue";
</script>
