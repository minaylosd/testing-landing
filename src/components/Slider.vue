<template>
  <section class="relative w-full my-16 overflow-hidden rounded-4xl">
    <Carousel
      :perPage="1"
      paginationActiveColor="#333"
      paginationPosition="top-overlay"
      autoplay="true"
    >
      <Slide v-for="(slide, index) in slides" :key="index" class="relative">
        <img class="rounded-4xl" :src="slide.image" :alt="slide.heading" />
        <div
          class="absolute top-0 left-0 grid grid-cols-2 px-10 pt-6 pb-8 my-6 min-h-35"
        >
          <div class="h-[300px] mb-6">
            <h1
              class="mb-4 font-medium leading-none text-white font-wide text-heading"
            >
              Тестирование продуктов «МТС»
            </h1>
            <p class="text-xl font-normal text-white font-compact">
              МТС постоянно выпускает новые диджитал-продукты, и вы можете
              сделать их удобнее. Находите баги, отправляйте отчёты об ошибках и
              получайте вознаграждение.
            </p>
          </div>

          <div class="flex items-center justify-between col-span-2">
            <a
              class="flex items-center p-2.5 text-xs font-bold tracking-wider uppercase font-wide text-txt rounded-2xl bg-white"
              href="/"
              ><span class="px-2 py-1">Войти</span></a
            >
          </div>
        </div>
      </Slide>
    </Carousel>
  </section>
</template>

<script setup>
import { ref } from "vue";
import { Carousel, Slide } from "vue-carousel";

const slides = ref([
  {
    image: "/carousel.jpg",
    heading: "Тестирование продуктов «МТС»",
    description:
      "МТС постоянно выпускает новые диджитал-продукты, и вы можете сделать их удобнее. Находите баги, отправляйте отчёты об ошибках и получайте вознаграждение.",
  },
  {
    image: "/carousel.jpg",
    heading: "Тестирование продуктов «МТС»",
    description:
      "МТС постоянно выпускает новые диджитал-продукты, и вы можете сделать их удобнее. Находите баги, отправляйте отчёты об ошибках и получайте вознаграждение.",
  },
  {
    image: "/carousel.jpg",
    heading: "Тестирование продуктов «МТС»",
    description:
      "МТС постоянно выпускает новые диджитал-продукты, и вы можете сделать их удобнее. Находите баги, отправляйте отчёты об ошибках и получайте вознаграждение.",
  },
]);
</script>

<style scoped>
.VueCarousel-pagination {
  position: absolute !important;
  top: 0 !important;
}
</style>
