<template>
  <footer class="w-full py-16 bg-tertiary">
    <div
      class="max-w-screen-sm px-5 mx-auto md:max-w-screen-md lg:max-w-screen-lg xl:max-w-screen-xl"
    >
      <div
        class="grid items-start w-full grid-cols-12 gap-x-0 gap-y-8 md:gap-x-8"
      >
        <div class="col-span-12 md:col-span-4">
          <h2 class="mb-4 text-xl font-bold leading-6 font-text text-txt">
            Портал МТС тестирование
          </h2>
          <p class="mb-4 text-base font-normal font-text text-txt">
            Получай промокоды и другие бонусы за поиск багов
          </p>
          <p
            class="mb-4 text-base font-normal font-text text-greyfooter max-w-100"
          >
            Портал МТС Тестирование предназначен для дистанционной работы с
            внутренними и внешники тестировщиками компании МТС.
          </p>
        </div>

        <ul
          class="flex flex-col col-span-12 gap-5 md:col-start-8 md:col-span-2 lg:col-start-9"
        >
          <li>
            <router-link
              to="/"
              class="text-base font-normal font-text text-greyfooter"
              >Главная</router-link
            >
          </li>
          <li>
            <router-link
              to="/"
              class="text-base font-normal font-text text-greyfooter"
              >Продукты</router-link
            >
          </li>
          <li>
            <router-link
              to="/"
              class="text-base font-normal font-text text-greyfooter"
              >Войти</router-link
            >
          </li>
        </ul>
        <ul
          class="flex flex-col col-span-12 gap-5 md:col-span-3 lg:col-span-2 max-w-65"
        >
          <li>
            <a
              class="text-base font-normal font-text text-greyfooter"
              href="/"
              target="_blank"
              >Магазин</a
            >
          </li>
          <li>
            <a
              class="text-base font-normal font-text text-greyfooter"
              href="/"
              target="_blank"
              >Акции</a
            >
          </li>
          <li>
            <a
              class="text-base font-normal font-text text-greyfooter"
              href="/"
              target="_blank"
              >Поддержка</a
            >
          </li>
          <li>
            <a
              class="text-base font-normal font-text text-greyfooter"
              href="/"
              target="_blank"
              >Согласие на обработку персональных данных</a
            >
          </li>
          <li>
            <a
              class="text-base font-normal font-text text-greyfooter"
              href="/"
              target="_blank"
              >Условия проведения акции</a
            >
          </li>
        </ul>
      </div>
      <div class="w-full bg-divider/50 h-[1px] my-[54px]"></div>
      <div class="grid items-start grid-cols-12 gap-8">
        <div class="col-span-12 md:col-span-3 lg:col-span-2">
          <h3 class="mb-4 text-base font-normal font-text text-txt">
            Социальные сети
          </h3>
          <div class="flex gap-4">
            <a href="/"><img src="/icons/vk.svg" alt="Vk Logo" /></a>
            <a href="/"><img src="/icons/ok.svg" alt="Ok Logo" /></a>
          </div>
        </div>

        <div class="col-span-12 md:col-span-3 lg:col-span-2">
          <h3 class="mb-4 text-base font-normal font-text text-txt">
            Приложение
          </h3>
          <div class="flex gap-4">
            <img src="/icons/footer-logo.svg" alt="MTS Logo" />
            <div class="flex flex-col text-base font-normal font-text text-txt">
              Мой МТС
              <a class="font-medium text-accent font-compact" href="/"
                >Скачать</a
              >
            </div>
          </div>
        </div>

        <div
          class="flex flex-wrap col-span-12 text-base font-normal md:col-span-3 md:col-start-8 lg:col-start-9 gap-x-2 gap-y-3 font-text text-greyfooter"
        >
          <div class="flex gap-2">
            <a href="/">Контакты</a>
            <span>·</span>
          </div>
          <div class="flex gap-2">
            <a class="whitespace-nowrap" href="/">Раскрытие информации</a>
            <span>·</span>
          </div>
          <div class="flex gap-2">
            <a class="whitespace-nowrap" href="/">Документы ПАО МТС</a>
            <span>·</span>
          </div>
          <div class="flex gap-2">
            <a class="whitespace-nowrap" href="/">Документы ПАО МТС</a>
            <span>·</span>
          </div>
          <a class="whitespace-nowrap" href="/">Комплаенс и деловая этика</a>
        </div>
      </div>

      <div
        class="flex flex-col items-start justify-between mt-8 text-base font-normal md:flex-row font-text text-greyfooter"
      >
        <p class="">© 2024 ПАО «МТС» Все права защищены</p>
        <p class="text-right">+18</p>
      </div>
    </div>
  </footer>
</template>
