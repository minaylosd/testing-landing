<template>
  <header
    class="fixed top-0 left-0 z-30 w-full bg-white shadow-shadow py-[9px]"
  >
    <div
      class="box-content flex items-center justify-between max-w-screen-xl px-20 mx-auto 2xl:px-10"
    >
      <router-link
        class="flex items-center gap-2.5 font-compact text-xl leading-6 text-txt font-normal"
        to="/"
        ><HeaderLogo />Тестирование</router-link
      >
      <div class="flex items-center gap-4">
        <router-link
          class="flex items-center p-2.5 text-17 leading-6 font-medium font-wide text-txt"
          to="/balance"
          ><span class="px-2 py-1">Поддержка</span></router-link
        >
        <router-link
          class="flex items-center p-2.5 text-xs font-bold tracking-wider uppercase font-wide text-white rounded-2xl bg-brand"
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
