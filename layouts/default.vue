<template>
  <div>
    <header>
      <div class="header-top">
        <div class="container">
          <div class="logo">
            <NuxtLink to="/">
              <logoSvg />
            </NuxtLink>
          </div>

          <ul class="header-top__category">
            <li><a href="#" style="color: #2D4872;" class="header-top__category-link">Цены </a></li>
            <li><a href="#" class="header-top__category-link">Услуги</a></li>
            <li><a href="#" class="header-top__category-link">Портфолио</a></li>
            <li><a href="#" class="header-top__category-link">Акции</a></li>
            <li>
              <a href="#" class="header-top__category-link">Преимущества</a>
            </li>
            <li><a href="#" class="header-top__category-link">Блог</a></li>
            <li><a href="#" class="header-top__category-link">Контакты</a></li>
          </ul>

          <ul class="header-top__weekday">
            <li>
              <a href="tel +72332222222">
                <callPhoneSvgVue />
                +7 (233) 222-22-22
              </a>
            </li>
            <li>
              <p>08:00 - 22:00, без выходных</p>
            </li>
          </ul>

          <ul class="header-top__messengers" >
            <li>
              <a href="#">
                <img
                  src="~/assets/images/svg/header_top_messenger_1.svg"
                  alt="header-top__messengers"
                />
              </a>
            </li>
            <li>
              <a href="#">
                <img
                  src="~/assets/images/svg/header_top_messenger_2.svg"
                  alt="header-top__messengers"
                />
              </a>
            </li>
            <li>
              <a href="#">
                <img
                  src="~/assets/images/svg/header_top_messenger_3.svg"
                  alt="header-top__messengers"
                />
              </a>
            </li>
          </ul>

          <div class="header-top__getPhone">
            <a href="tel +72332222222">
                <callPhoneSvgVue v-if="false"/>
                Заказать звонок
            </a>
          </div>
        </div>
      </div>

      <div class="header-bottom">
        <ul class="header-bottom__category"></ul>
      </div>
    </header>

    <footer></footer>
  </div>
</template>

<script setup>
// import icon's
import logoSvg from "~/component/icon/logo.vue";
import callPhoneSvgVue from "~/component/icon/callPhoneSvg.vue";
</script>

<style lang="scss" scoped></style>
