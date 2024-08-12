<template>
  <section
    class="relative w-full mt-10 mb-10 overflow-hidden md:mt-16 md:mb-16 md:rounded-4xl rounded-2xl"
  >
    <Carousel
      :perPage="1"
      paginationActiveColor="rgba(0,0,0,1)"
      paginationColor="rgba(0,0,0,.2)"
      paginationPosition="top-overlay"
      :autoplay="true"
      :autoplayTimeout="5000"
    >
      <Slide
        v-for="(slide, index) in slides"
        :key="index"
        class="relative overflow-hidden min-h-[468px] h-[60vh] md:h-auto rounded-2xl md:rounded-4xl"
      >
        <img
          class="absolute top-0 left-0 object-cover md:w-full w-full md:h-inherit h-full md:rounded-4xl rounded-2xl max-w-[200vw] overflow-hidden"
          :src="slide.image"
          :alt="slide.heading"
        />

        <div
          class="relative top-0 left-0 grid grid-cols-1 px-5 pb-8 pt-13 md:px-10 lg:grid-cols-2 min-h-35"
        >
          <div class="md:h-[300px] xl:mb-6 mb-4">
            <h1
              class="mb-4 text-3xl font-medium text-white md:leading-none font-wide lg:text-heading"
            >
              Тестирование продуктов «МТС»
            </h1>
            <p class="text-xl font-normal text-white font-compact">
              МТС постоянно выпускает новые диджитал-продукты, и вы можете
              сделать их удобнее. Находите баги, отправляйте отчёты об ошибках и
              получайте вознаграждение.
            </p>
          </div>

          <div
            class="flex items-center justify-between mt-6 lg:col-span-2 md:mt-0"
          >
            <a
              class="flex items-center p-3.5 text-xl font-regular leading-4 tracking-wider font-text text-txt rounded-2xl bg-white"
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

// // Define the method to be called when the transition ends
// const onTransitionEnd = () => {
//   animateIndicator();
// };

// // Define the function to change the color from left to right
// const animateIndicator = () => {
//   const element = document.querySelector(".VueCarousel-dot--active");
//   if (element) {
//     // Example of changing color from left to right
//     element.style.background =
//       "linear-gradient(to right, rgba(0,0,0,1) 100%, rgba(0,0,0,.2) 101%)";
//   }
// };
</script>

<style>
.VueCarousel-dot-container {
  width: 100% !important;
  display: flex !important;
  flex-wrap: nowrap !important;
  align-items: center !important;
  gap: 8px !important;
  padding: 0 20px !important;
  margin: 24px auto !important;
}

.VueCarousel-dot {
  width: 100% !important;
  height: 4px !important;
  border-radius: 0 !important;
  padding: 0 !important;
  border-radius: 5px !important;
  margin: 0 !important;
  transition: all 0.3s ease-in-out;
  border: none !important;
}
</style>
