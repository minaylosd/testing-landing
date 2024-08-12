<script setup>
import { ref, computed } from "vue";
import Slider from "../components/Slider.vue";
import AccordeonCard from "../components/AccordeonCard.vue";
</script>
<template>
  <main
    class="max-w-screen-sm px-5 mx-auto md:max-w-screen-md xl:max-w-screen-xl lg:max-w-screen-lg xl:mt-17 mt-13"
  >
    <Slider />

    <section class="grid grid-cols-1 gap-5 mb-10 md:mb-16 md:grid-cols-3">
      <div class="w-full p-4 bg-white rounded-3xl">
        <img class="mb-16 w-17 h-17" src="/icons/star.svg" alt="" />
        <h3 class="mb-2 text-xl font-medium leading-6 text-txt font-wide">
          Получайте промокоды и бонусы за поиск багов
        </h3>
        <p class="text-sm font-regular text-txt font-text">
          МТС постоянно выпускает новые диджитал-продукты, и вы можете сделать
          их удобнее. Находите баги, отправляйте отчёты об ошибках и получайте
          вознаграждение.
        </p>
      </div>

      <div class="w-full p-4 bg-white rounded-3xl">
        <img class="mb-16 w-17 h-17" src="/icons/star.svg" alt="" />
        <h3 class="mb-2 text-xl font-medium leading-6 text-txt font-wide">
          Получайте промокоды и бонусы за поиск багов
        </h3>
        <p class="text-sm font-regular text-txt font-text">
          МТС постоянно выпускает новые диджитал-продукты, и вы можете сделать
          их удобнее. Находите баги, отправляйте отчёты об ошибках и получайте
          вознаграждение.
        </p>
      </div>

      <div class="w-full p-4 bg-white rounded-3xl">
        <img class="mb-16 w-17 h-17" src="/icons/star.svg" alt="" />
        <h3 class="mb-2 text-xl font-medium leading-6 text-txt font-wide">
          Получайте промокоды и бонусы за поиск багов
        </h3>
        <p class="text-sm font-regular text-txt font-text">
          МТС постоянно выпускает новые диджитал-продукты, и вы можете сделать
          их удобнее. Находите баги, отправляйте отчёты об ошибках и получайте
          вознаграждение.
        </p>
      </div>
    </section>

    <section class="mb-10 md:mb-16">
      <h1
        class="mb-4 text-2xl font-medium md:mb-8 md:text-4xl leading-13 text-txt font-wide"
      >
        С нами стали лучше
      </h1>
      <div
        class="grid items-center justify-center grid-cols-2 gap-5 md:grid-cols-3 lg:flex"
      >
        <div
          class="lg:w-[190px] w-full h-[90px] rounded-4xl border border-divider flex items-center justify-center"
        >
          <img
            class="w-4/6 xl:w-auto md:w-3/4"
            src="/icons/vkLogo.png"
            alt="VK logo"
          />
        </div>

        <div
          class="lg:w-[190px] w-full h-[90px] rounded-4xl border border-divider flex items-center justify-center"
        >
          <img
            class="w-4/6 xl:w-auto lg:w-3/4"
            src="/icons/spotifyLogo.png"
            alt="Spotify logo"
          />
        </div>

        <div
          class="lg:w-[190px] w-full h-[90px] rounded-4xl border border-divider flex items-center justify-center"
        >
          <img
            class="w-4/6 xl:w-auto lg:w-3/4"
            src="/icons/vkLogo.png"
            alt="VK logo"
          />
        </div>

        <div
          class="lg:w-[190px] w-full h-[90px] rounded-4xl border border-divider flex items-center justify-center"
        >
          <img class="w-auto" src="/icons/okLogo.png" alt="OK logo" />
        </div>

        <div
          class="lg:w-[190px] w-full h-[90px] rounded-4xl border border-divider flex items-center justify-center"
        >
          <img
            class="w-4/6 xl:w-auto lg:w-3/4"
            src="/icons/spotifyLogo.png"
            alt="Spotify logo"
          />
        </div>

        <div
          class="lg:w-[190px] w-full h-[90px] rounded-4xl border border-divider flex items-center justify-center"
        >
          <img
            class="w-4/6 xl:w-auto lg:w-3/4"
            src="/icons/vkLogo.png"
            alt="VK logo"
          />
        </div>
      </div>
    </section>

    <AccordeonCard />
  </main>
</template>
