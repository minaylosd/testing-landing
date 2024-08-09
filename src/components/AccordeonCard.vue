<template>
  <section class="bg-white rounded-[60px] p-16 mb-16">
    <h1 class="mb-8 text-4xl font-medium leading-13 text-txt font-wide">
      Часто задаваемые вопросы
    </h1>
    <div class="flex flex-col gap-5">
      <div
        v-for="(item, index) in faqItems"
        :key="index"
        class="flex flex-col items-start justify-between w-full overflow-hidden border-b border-divider"
      >
        <div
          :class="isOpen(index) ? 'h-auto' : 'max-h-12'"
          class="flex items-start justify-between w-full pb-5 transition-all duration-500 cursor-pointer"
          @click="toggleAccordion(index)"
        >
          <div class="max-w-[630px]">
            <h3 class="mb-3 text-xl font-medium text-txt font-wide">
              {{ item.question }}
            </h3>
            <p
              :class="isOpen(index) ? 'opacity-100 h-auto' : 'opacity-0 h-0'"
              class="leading-6 transition-opacity duration-500 opacity-0 text-17 font-regular text-greytxt font-text"
            >
              {{ item.answer }}
            </p>
          </div>
          <div
            :class="isOpen(index) ? 'rotate-180' : ''"
            class="transition-transform duration-500 ease-in-out"
          >
            <img
              src="/icons/chevron.svg"
              alt=""
              class="transition-transform duration-500"
            />
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref } from "vue";

const faqItems = ref([
  {
    question: "Какое вознаграждение за тестирование продуктов?",
    answer:
      "Вознаграждение за успешное тестирование продуктов вы сможете выбрать в нашем магазине вознаграждений.",
  },
  {
    question: "Какие продукты я смогу протестировать?",
    answer:
      "Вознаграждение за успешное тестирование продуктов вы сможете выбрать в нашем магазине вознаграждений.",
  },
  {
    question: "Какие продукты вы уже протестировали?",
    answer:
      "Вознаграждение за успешное тестирование продуктов вы сможете выбрать в нашем магазине вознаграждений.",
  },
]);

const openIndex = ref(null);

const toggleAccordion = (index) => {
  openIndex.value = openIndex.value === index ? null : index;
};

const isOpen = (index) => {
  return openIndex.value === index;
};
</script>
