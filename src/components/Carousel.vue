<template>
  <section
    class="w-full mt-10 mb-10 overflow-hidden md:mt-16 md:mb-16 md:rounded-4xl rounded-2xl"
  >
    <swiper class="w-full swiper" :options="swiperOptions">
      <swiper-slide
        style="width: auto !important"
        class="relative overflow-hidden min-h-[468px] h-[60vh] md:h-auto rounded-2xl md:rounded-4xl w-full"
      >
        <a class="w-full" href="/">
          <img
            class="absolute top-0 left-0 object-cover md:w-full w-full md:h-inherit h-full md:rounded-4xl rounded-2xl max-w-[200vw]"
            src="/carousel.jpg"
            alt="slide.heading"
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
                сделать их удобнее. Находите баги, отправляйте отчёты об ошибках
                и получайте вознаграждение.
              </p>
            </div>
            <div
              class="flex items-center justify-between mt-6 lg:col-span-2 md:mt-0"
            >
              <a
                class="flex items-center p-3.5 text-xl font-regular leading-4 tracking-wider font-text text-txt rounded-2xl bg-white"
                href="/"
              >
                <span class="px-2 py-1">Войти</span>
              </a>
            </div>
          </div></a
        >
      </swiper-slide>

      <swiper-slide
        style="width: auto !important"
        class="relative overflow-hidden min-h-[468px] w-full h-[60vh] md:h-auto rounded-2xl md:rounded-4xl"
      >
        <a href="/"
          ><img
            class="absolute top-0 left-0 object-cover md:w-full w-full md:h-inherit h-full md:rounded-4xl rounded-2xl max-w-[200vw]"
            src="/carousel.jpg"
            alt="slide.heading"
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
                сделать их удобнее. Находите баги, отправляйте отчёты об ошибках
                и получайте вознаграждение.
              </p>
            </div>
            <div
              class="flex items-center justify-between mt-6 lg:col-span-2 md:mt-0"
            >
              <a
                class="flex items-center p-3.5 text-xl font-regular leading-4 tracking-wider font-text text-txt rounded-2xl bg-white"
                href="/"
              >
                <span class="px-2 py-1">Войти</span>
              </a>
            </div>
          </div></a
        >
      </swiper-slide>

      <swiper-slide
        style="width: auto !important"
        class="relative overflow-hidden min-h-[468px] w-full h-[60vh] md:h-auto rounded-2xl md:rounded-4xl"
      >
        <a href="/"
          ><img
            class="absolute top-0 left-0 object-cover md:w-full w-full md:h-inherit h-full md:rounded-4xl rounded-2xl max-w-[200vw]"
            src="/carousel.jpg"
            alt="slide.heading"
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
                сделать их удобнее. Находите баги, отправляйте отчёты об ошибках
                и получайте вознаграждение.
              </p>
            </div>
            <div
              class="flex items-center justify-between mt-6 lg:col-span-2 md:mt-0"
            >
              <a
                class="flex items-center p-3.5 text-xl font-regular leading-4 tracking-wider font-text text-txt rounded-2xl bg-white"
                href="/"
              >
                <span class="px-2 py-1">Войти</span>
              </a>
            </div>
          </div></a
        >
      </swiper-slide>
      <div class="swiper-pagination" slot="pagination"></div>
    </swiper>
  </section>
</template>

<script setup>
import { ref, onMounted } from "vue";
import { Swiper, SwiperSlide } from "vue-awesome-swiper";
import "swiper/css/swiper.css";

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

const swiperOptions = ref({
  slidesPerView: 1,
  spaceBetween: 20,
  loop: true,
  speed: 800,
  autoplay: {
    delay: 5000,
    disableOnInteraction: false,
  },
  pagination: {
    el: ".swiper-pagination",
    clickable: true,
  },
  breakpoints: {
    360: {
      slidesPerView: 1,
      spaceBetween: 20,
    },
    // when window width is >= 640px
    640: {
      slidesPerView: 1,
      spaceBetween: 20,
    },
    // when window width is >= 768px
    768: {
      slidesPerView: 1,
      spaceBetween: 30,
    },
    // when window width is >= 1024px
    1024: {
      slidesPerView: 1,
      spaceBetween: 40,
    },
    // Add more breakpoints as needed
  },
});
onMounted(() => {
  const swiper = document.querySelector(".swiper").swiper;

  // Forcefully override widths on all slides
  swiper.slides.forEach((slide) => {
    slide.style.width = "auto";
    slide.style.maxWidth = "100%";
  });

  swiper.update(); // Update swiper to apply new widths
});
</script>

<style>
.swiper-slide {
  width: 100% !important; /* Adjusting for padding */
  max-width: 100% !important;
  min-width: 100% !important; /* Force minimum width */
}
.swiper-pagination {
  width: 100% !important;
  height: 4px;
  display: flex !important;
  flex-wrap: nowrap !important;
  align-items: center !important;
  gap: 8px !important;
  padding: 0 20px !important;
  margin: 24px auto !important;
  position: absolute;
  top: 0;
  left: 0;
}

.swiper-pagination-bullet {
  width: 100% !important;
  height: 4px !important;
  border-radius: 5px !important;
  background-color: rgba(0, 0, 0, 0.2) !important;
  overflow: hidden;
  position: relative;
  opacity: 100% !important;
}

.swiper-pagination-bullet-active::after {
  content: "";
  width: 0%;
  height: 100%;
  display: block;
  background-color: rgba(0, 0, 0, 1);
  animation: moveLine 5.8s forwards linear;
}

@keyframes moveLine {
  from {
    width: 0;
  }
  to {
    width: 100%;
  }
}
</style>
