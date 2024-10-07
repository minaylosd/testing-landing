<script setup>
import AccordeonCard from "../components/AccordeonCard.vue";
import Carousel from "../components/Carousel.vue";
</script>
<template>
  <main
    class="max-w-screen-sm px-5 mx-auto md:max-w-screen-md xl:max-w-screen-xl lg:max-w-screen-lg xl:mt-17 mt-13"
  >
    <Carousel />

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
        data-animation="ticker__wrapper"
        class="relative flex w-full overflow-hidden h-[90px]"
      >
        <div
          data-animation="ticker"
          class="flex flex-nowrap gap-5 absolute top-0 left-0 w-fit h-[90px]"
        >
          <div class="flex items-center justify-center gap-5">
            <div
              class="w-[190px] h-[90px] rounded-4xl border border-divider flex items-center justify-center"
            >
              <img class="w-auto" src="/icons/okLogo.png" alt="OK logo" />
            </div>

            <div
              class="w-[190px] h-[90px] rounded-4xl border border-divider flex items-center justify-center"
            >
              <img
                class="w-3/4 xl:w-auto"
                src="/icons/spotifyLogo.png"
                alt="Spotify logo"
              />
            </div>

            <div
              class="w-[190px] h-[90px] rounded-4xl border border-divider flex items-center justify-center"
            >
              <img
                class="w-3/4 xl:w-auto"
                src="/icons/vkLogo.png"
                alt="VK logo"
              />
            </div>

            <div
              class="w-[190px] h-[90px] rounded-4xl border border-divider flex items-center justify-center"
            >
              <img
                class="w-4/6 md:w-3/4"
                src="/icons/Verse logo.png"
                alt="MTS Verse logo"
              />
            </div>

            <div
              class="w-[190px] h-[90px] rounded-4xl border border-divider flex items-center justify-center"
            >
              <img
                class="w-3/4"
                src="/icons/Membrana Kids.png"
                alt="Membrana Kids logo"
              />
            </div>

            <div
              class="w-[190px] h-[90px] rounded-4xl border border-divider flex items-center justify-center"
            >
              <img class="w-3/4" src="/icons/NUUM.png" alt="NUUM logo" />
            </div>

            <div
              class="w-[190px] h-[90px] rounded-4xl border border-divider flex items-center justify-center"
            >
              <img
                class="w-4/6 xl:w-auto md:w-3/4"
                src="/icons/MTS stroki.png"
                alt="MTS Строки logo"
              />
            </div>

            <div
              class="w-[190px] h-[90px] rounded-4xl border border-divider flex items-center justify-center"
            >
              <img
                class="w-4/6 xl:w-auto md:w-3/4"
                src="/icons/MTS auto.png"
                alt="MTS Авто logo"
              />
            </div>

            <div
              class="w-[190px] h-[90px] rounded-4xl border border-divider flex items-center justify-center"
            >
              <img
                class="w-4/6 xl:w-auto md:w-3/4"
                src="/icons/tododo.png"
                alt="Тудуду logo"
              />
            </div>

            <div
              class="w-[190px] h-[90px] rounded-4xl border border-divider flex items-center justify-center"
            >
              <img
                class="w-4/6 xl:w-auto md:w-3/4"
                src="/icons/MTS smart home.png"
                alt="MTS Умный дом logo"
              />
            </div>
          </div>

          <div class="flex items-center justify-center gap-5">
            <div
              class="w-[190px] h-[90px] rounded-4xl border border-divider flex items-center justify-center"
            >
              <img class="w-auto" src="/icons/okLogo.png" alt="OK logo" />
            </div>

            <div
              class="w-[190px] h-[90px] rounded-4xl border border-divider flex items-center justify-center"
            >
              <img
                class="w-3/4 xl:w-auto"
                src="/icons/spotifyLogo.png"
                alt="Spotify logo"
              />
            </div>

            <div
              class="w-[190px] h-[90px] rounded-4xl border border-divider flex items-center justify-center"
            >
              <img
                class="w-3/4 xl:w-auto"
                src="/icons/vkLogo.png"
                alt="VK logo"
              />
            </div>

            <div
              class="w-[190px] h-[90px] rounded-4xl border border-divider flex items-center justify-center"
            >
              <img
                class="w-4/6 md:w-3/4"
                src="/icons/Verse logo.png"
                alt="MTS Verse logo"
              />
            </div>

            <div
              class="w-[190px] h-[90px] rounded-4xl border border-divider flex items-center justify-center"
            >
              <img
                class="w-3/4"
                src="/icons/Membrana Kids.png"
                alt="Membrana Kids logo"
              />
            </div>

            <div
              class="w-[190px] h-[90px] rounded-4xl border border-divider flex items-center justify-center"
            >
              <img class="w-3/4" src="/icons/NUUM.png" alt="NUUM logo" />
            </div>

            <div
              class="w-[190px] h-[90px] rounded-4xl border border-divider flex items-center justify-center"
            >
              <img
                class="w-4/6 xl:w-auto md:w-3/4"
                src="/icons/MTS stroki.png"
                alt="MTS Строки logo"
              />
            </div>

            <div
              class="w-[190px] h-[90px] rounded-4xl border border-divider flex items-center justify-center"
            >
              <img
                class="w-4/6 xl:w-auto md:w-3/4"
                src="/icons/MTS auto.png"
                alt="MTS Авто logo"
              />
            </div>

            <div
              class="w-[190px] h-[90px] rounded-4xl border border-divider flex items-center justify-center"
            >
              <img
                class="w-4/6 xl:w-auto md:w-3/4"
                src="/icons/tododo.png"
                alt="Тудуду logo"
              />
            </div>

            <div
              class="w-[190px] h-[90px] rounded-4xl border border-divider flex items-center justify-center"
            >
              <img
                class="w-4/6 xl:w-auto md:w-3/4"
                src="/icons/MTS smart home.png"
                alt="MTS Умный дом logo"
              />
            </div>
          </div>
        </div>
      </div>
    </section>

    <AccordeonCard />
  </main>
</template>

<style scoped>
div[data-animation="ticker"] {
  animation: ticker 25s linear infinite;
}

div[data-animation="ticker__wrapper"] {
  mask-image: linear-gradient(
    to right,
    transparent,
    black 2%,
    black 98%,
    transparent
  );
  mask-size: 100% 100%;
  mask-repeat: no-repeat;
}

@keyframes ticker {
  0% {
    transform: translateX(0);
  }
  100% {
    transform: translateX(calc(-50% - 10px));
  }
}
</style>
