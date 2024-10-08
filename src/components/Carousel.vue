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
            class="absolute top-0 left-0 object-cover w-full h-auto md:w-auto md:h-full md:rounded-4xl rounded-2xl max-w-[200vw]"
            :src="bannerSrc"
            alt="slide.heading"
          />
        </a>
      </swiper-slide>

      <swiper-slide
        style="width: auto !important"
        class="relative overflow-hidden min-h-[468px] h-[60vh] md:h-auto rounded-2xl md:rounded-4xl w-full"
      >
        <a class="w-full" href="/">
          <img
            class="absolute top-0 left-0 object-cover w-full h-auto md:w-auto md:h-full md:rounded-4xl rounded-2xl max-w-[200vw]"
            :src="bannerSrc"
            alt="slide.heading"
          />
        </a>
      </swiper-slide>

      <swiper-slide
        style="width: auto !important"
        class="relative overflow-hidden min-h-[468px] h-[60vh] md:h-auto rounded-2xl md:rounded-4xl w-full"
      >
        <a class="w-full" href="/">
          <img
            class="absolute top-0 left-0 object-cover w-full h-auto md:w-auto md:h-full md:rounded-4xl rounded-2xl max-w-[200vw]"
            :src="bannerSrc"
            alt="slide.heading"
          />
        </a>
      </swiper-slide>

      <div class="swiper-pagination" slot="pagination"></div>
    </swiper>
  </section>
</template>

<script setup>
import { ref, onMounted, onBeforeUnmount, computed } from "vue";
import { Swiper, SwiperSlide } from "vue-awesome-swiper";
import "swiper/css/swiper.css";

const windowWidth = ref(window.innerWidth);

const handleResize = () => {
  windowWidth.value = window.innerWidth;
};

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
  window.addEventListener("resize", handleResize);
});

onBeforeUnmount(() => {
  window.removeEventListener("resize", handleResize);
});

const bannerSrc = computed(() => {
  return windowWidth.value < 768 ? "/banner-mob.png" : "/banner-desktop.png";
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
