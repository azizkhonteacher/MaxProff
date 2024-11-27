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
            <li>
              <a
                href="#"
                style="color: #2d4872"
                class="header-top__category-link"
                >Цены
              </a>
            </li>
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

          <ul class="header-top__messengers">
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
              <callPhoneSvgVue v-if="false" />
              Заказать звонок
            </a>
          </div>
        </div>
      </div>

      <div class="header-bottom">
        <div class="container">
          <ul class="header-bottom__category-list">
            <!-- list-1 -->
            <li class="header-bottom__category">
              <div class="header-bottom__category-title">
                <p>Ремонт квартир</p>
                <chevronDownSvg />
              </div>

              <ul>
                <li><a href="#">Подпункт</a></li>
                <li><a href="#">Подпункт</a></li>
                <li><a href="#">Акции</a></li>
                <li><a href="#">Преимущества</a></li>
                <li><a href="#">Контакты</a></li>
              </ul>
            </li>
            <!-- list-2 -->
            <li class="header-bottom__category">
              <div class="header-bottom__category-title">
                <p>Ремонт квартир</p>
                <chevronDownSvg />
              </div>

              <ul>
                <li><a href="#">Подпункт</a></li>
                <li><a href="#">Подпункт</a></li>
                <li><a href="#">Акции</a></li>
                <li><a href="#">Преимущества</a></li>
                <li><a href="#">Контакты</a></li>
              </ul>
            </li>
            <!-- list-3 -->
            <li class="header-bottom__category">
              <div class="header-bottom__category-title">
                <p>Ремонт квартир</p>
                <chevronDownSvg />
              </div>

              <ul>
                <li><a href="#">Подпункт</a></li>
                <li><a href="#">Подпункт</a></li>
                <li><a href="#">Акции</a></li>
                <li><a href="#">Преимущества</a></li>
                <li><a href="#">Контакты</a></li>
              </ul>
            </li>
            <!-- list-4 -->
            <li class="header-bottom__category">
              <div class="header-bottom__category-title">
                <a href="#">Ремонт квартир</a>
              </div>
            </li>
            <!-- list-5 -->
            <li class="header-bottom__category">
              <div class="header-bottom__category-title">
                <a href="#">Ремонт квартир</a>
              </div>
            </li>
          </ul>
        </div>
      </div>
    </header>

    <main>
      <NuxtPage />
    </main>

    <footer>
      <div class="footer-top">
        <div class="container">
          <h2 class="footer-top__title">Нужна консультация?</h2>
          <p class="footer-top__desc">
            Подробно расскажем о наших услугах, видах работ и типовых проектах,
            рассчитаем стоимость и подготовим индивидуальное предложение!
          </p>
          <button class="footer-top__btn">Оставить заявку</button>
        </div>
      </div>

      <div class="footer-bottom">
        <div class="footer-bottom__top">
          <div class="container">
            <ul class="footer-bottom__top-list">
              <!-- logo list -->
              <li class="logo-list">
                <div class="logo">
                  <NuxtLink to="/">
                    <logoSvg />
                  </NuxtLink>
                </div>

                <div class="panments">
                  <p>Любая форма оплаты</p>
                  <ul class="panments-ul">
                    <!-- wallet-1 -->
                    <li>
                      <img
                        src="~/assets/images/wallet/wallet-1.svg"
                        alt="wallet img"
                      />
                    </li>
                    <!-- wallet-2 -->
                    <li>
                      <img
                        src="~/assets/images/wallet/wallet-2.svg"
                        alt="wallet img"
                      />
                    </li>
                    <!-- wallet-3 -->
                    <li>
                      <img
                        src="~/assets/images/wallet/wallet-3.svg"
                        alt="wallet img"
                      />
                    </li>
                    <!-- wallet-4 -->
                    <li>
                      <img
                        src="~/assets/images/wallet/wallet-4.svg"
                        alt="wallet img"
                      />
                    </li>
                    <!-- wallet-5 -->
                    <li>
                      <img
                        src="~/assets/images/wallet/wallet-5.svg"
                        alt="wallet img"
                      />
                    </li>
                  </ul>
                </div>

                <ul class="messengers" v-if="false">
                  <li>
                    <NuxtLink to="/">
                      <img
                        src="~/assets/images/icon/facebook.svg"
                        alt="messengers"
                      />
                    </NuxtLink>
                  </li>
                  <li>
                    <NuxtLink to="/">
                      <img
                        src="~/assets/images/icon/youtobe.svg"
                        alt="messengers"
                      />
                    </NuxtLink>
                  </li>
                  <li>
                    <NuxtLink to="/">
                      <img
                        src="~/assets/images/icon/instagram.svg"
                        alt="messengers"
                      />
                    </NuxtLink>
                  </li>
                  <li>
                    <NuxtLink to="/">
                      <img
                        src="~/assets/images/icon/telegram.svg"
                        alt="messengers"
                      />
                    </NuxtLink>
                  </li>
                  <li>
                    <NuxtLink to="/">
                      <img
                        src="~/assets/images/icon/Vector.svg"
                        alt="messengers"
                      />
                    </NuxtLink>
                  </li>
                  <li>
                    <NuxtLink to="/">
                      <img
                        src="~/assets/images/icon/odnoklassniki.svg"
                        alt="messengers"
                      />
                    </NuxtLink>
                  </li>
                </ul>
              </li>

              <!-- Our services -->
              <li class="ourServices">
                <h3 class="ourServices-title">Наши услуги</h3>

                <ul class="ourServices-list">
                  <li>Квартиры</li>
                  <li>Коттеджи</li>
                  <li>Таунхаусы</li>
                  <li>Офисы</li>
                  <li>Инженерные системы</li>
                  <li>География работ</li>
                </ul>
              </li>

              <!-- footer categorys -->
              <li class="categorys">
                <ul class="categorys-list">
                  <li><NuxtLink to="/">Портфолио</NuxtLink></li>
                  <li><NuxtLink to="/">Стоимость</NuxtLink></li>
                  <li><NuxtLink to="/">Акции</NuxtLink></li>
                  <li><NuxtLink to="/">О компании</NuxtLink></li>
                  <li><NuxtLink to="/">Статьи</NuxtLink></li>
                  <li><NuxtLink to="/">Контакты</NuxtLink></li>
                </ul>
              </li>

              <!-- connect -->
              <li class="connect">
                <ul class="connect-list">
                  <!-- tel -->
                  <li class="connect-tel">
                    <NuxtLink to="tel +72332222222">
                      <callPhoneSvgVue />
                      <div class="desc">
                        <h4>+7 (233) 222-22-22</h4>
                        <p>08:00 - 22:00, без выходных</p>
                        <span>Заказать звонок</span>
                      </div>
                    </NuxtLink>
                  </li>

                  <!-- email -->
                  <li>
                    <NuxtLink to="/">
                      <mailSvg />
                      <p>Электронная почта @</p>
                    </NuxtLink>
                  </li>

                  <!-- location -->
                  <li>
                    <NuxtLink to="/">
                      <locationSvg />
                      <p>Адрес</p>
                    </NuxtLink>
                  </li>
                </ul>
              </li>
            </ul>
          </div>
        </div>
        <!-- bottom bottom -->
        <div class="footer-bottom__sub">
          <div class="container">
            <!-- info -->
            <h2 class="info">
              &copy; 2021 «MaxProff»
              <NuxtLink to="/">Правовая информация</NuxtLink>
            </h2>
            <!-- messengers -->
            <ul class="messengers">
              <li>
                <NuxtLink to="/">
                  <img
                    src="~/assets/images/icon/facebook.svg"
                    alt="messengers"
                  />
                </NuxtLink>
              </li>
              <li>
                <NuxtLink to="/">
                  <img
                    src="~/assets/images/icon/youtobe.svg"
                    alt="messengers"
                  />
                </NuxtLink>
              </li>
              <li>
                <NuxtLink to="/">
                  <img
                    src="~/assets/images/icon/instagram.svg"
                    alt="messengers"
                  />
                </NuxtLink>
              </li>
              <li>
                <NuxtLink to="/">
                  <img
                    src="~/assets/images/icon/telegram.svg"
                    alt="messengers"
                  />
                </NuxtLink>
              </li>
              <li>
                <NuxtLink to="/">
                  <img src="~/assets/images/icon/Vector.svg" alt="messengers" />
                </NuxtLink>
              </li>
              <li>
                <NuxtLink to="/">
                  <img
                    src="~/assets/images/icon/odnoklassniki.svg"
                    alt="messengers"
                  />
                </NuxtLink>
              </li>
            </ul>

            <!-- desc -->
            <p class="desc">
              Сайт не является публичной офертой и носит информационный характер
            </p>

            <NuxtLink class="carta" to="/">Карта сайта</NuxtLink>
          </div>
        </div>
      </div>
    </footer>
  </div>
</template>

<script setup>
// import icon's
import logoSvg from "~/component/icon/logo.vue";
import callPhoneSvgVue from "~/component/icon/callPhoneSvg.vue";
import chevronDownSvg from "~/component/icon/chevronDownSvg.vue";
import mailSvg from "~/component/icon/mailSvg.vue";
import locationSvg from "~/component/icon/locationSvg.vue";
</script>

<style lang="scss" scoped></style>
