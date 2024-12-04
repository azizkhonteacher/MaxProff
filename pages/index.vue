<template>
  <div>
    <div class="hero">
      <div class="container">
        <div class="hero__info-wrap">
          <!-- hero title -->
          <h2 class="hero__info-title">РЕМОНТ КВАРТИР В МОСКВЕ И МО</h2>
          <!-- hero sub title -->
          <h3 class="hero__info-sub-title">от <span>2450</span> руб/м2</h3>

          <div class="convenience-wrap">
            <!-- card-1 -->
            <div class="convenience-card">
              <div class="convenience-card__img">
                <img
                  src="~/assets/images/svg/hero-work-img-1.svg"
                  alt="wroks skills"
                />
                <span></span>
              </div>
              <p>
                Оплата по факту <br />
                приема работ
              </p>
            </div>
            <!-- card-2 -->
            <div class="convenience-card">
              <div class="convenience-card__img">
                <img
                  src="~/assets/images/svg/hero-work-img-2.svg"
                  alt="wroks skills"
                />
                <span></span>
              </div>
              <p>Замер и составление сметы БЕСПЛАТНО</p>
            </div>
            <!-- card-3 -->
            <div class="convenience-card">
              <div class="convenience-card__img">
                <img
                  src="~/assets/images/svg/hero-work-img-3.svg"
                  alt="wroks skills"
                />
                <span></span>
              </div>
              <p>Выезд сметчика</p>
            </div>
            <!-- card-4 -->
            <div class="convenience-card">
              <div class="convenience-card__img">
                <img
                  src="~/assets/images/svg/hero-work-img-4.svg"
                  alt="wroks skills"
                />
                <span></span>
              </div>
              <p>Гарантия 3 года</p>
            </div>
          </div>
        </div>

        <div class="repair__calculate">
          <h2 class="repair__calculate-title">РАССЧИТАЙТЕ стоимость ремонта</h2>

          <form class="repair__calculate-form">
            <div class="repair__calculate-form-check-inputs">
              <!--        repair type check inputs   item         -->
              <div class="repair__calculate-form-item repair-type">
                <h2 class="title">Вид ремонта:</h2>
                <!--                inputs wrapper       -->
                <div class="grid grid-cols-2 w-full gap-y-2.5 gap-x-px">
                  <!-- 1 -->
                  <div class="flex justify-start w-full items-center gap-2.5">
                    <input
                      id="i1"
                      name="repair-type"
                      type="radio"
                      value="Косметический"
                    />
                    <label for="i1">Косметический</label>
                  </div>
                  <!-- 2 -->
                  <div class="flex justify-start w-full items-center gap-2.5">
                    <input
                      id="i2"
                      name="repair-type"
                      type="radio"
                      value="Капитальный"
                    />
                    <label for="i2">Капитальный</label>
                  </div>
                  <!-- 3 -->
                  <div class="flex justify-start w-full items-center gap-2.5">
                    <input
                      id="i3"
                      name="repair-type"
                      type="radio"
                      value="Под ключ"
                    />
                    <label for="i3">Под ключ</label>
                  </div>
                  <!-- 4 -->
                  <div class="flex justify-start w-full items-center gap-2.5">
                    <input
                      id="i4"
                      name="repair-type"
                      type="radio"
                      value="Дизайнерский"
                    />
                    <label for="i4">Дизайнерский</label>
                  </div>
                </div>
              </div>

              <!--        property type check inputs   item         -->
              <div class="repair__calculate-form-item property-type">
                <h2 class="title">Тип вашей недвижимости:</h2>
                <!--                inputs wrapper       -->
                <div class="grid grid-cols-2 w-full gap-y-2.5 gap-x-px">
                  <!-- 1 -->
                  <div class="flex justify-start w-full items-center gap-2.5">
                    <input
                      id="p1"
                      name="property-type"
                      type="radio"
                      value="Новостройка"
                    />
                    <label for="p1">Новостройка</label>
                  </div>
                  <!-- 2 -->
                  <div class="flex justify-start w-full items-center gap-2.5">
                    <input
                      id="p2"
                      name="property-type"
                      type="radio"
                      value="Вторичное жилье"
                    />
                    <label for="p2">Вторичное жилье</label>
                  </div>
                </div>
              </div>

              <!--        number-room type check inputs   item         -->
              <div class="repair__calculate-form-item number-room">
                <h2 class="title">Количество комнат</h2>
                <!--                inputs wrapper       -->
                <div class="flex items-center gap-x-6">
                  <!-- 1 -->
                  <div class="flex items-center gap-2.5">
                    <input id="r1" name="number-room" type="radio" value="1" />
                    <label for="r1">1</label>
                  </div>
                  <!-- 2 -->
                  <div class="flex items-center gap-2.5">
                    <input id="r2" name="number-room" type="radio" value="2" />
                    <label for="r2">2</label>
                  </div>
                  <!-- 3 -->
                  <div class="flex items-center gap-2.5">
                    <input id="r3" name="number-room" type="radio" value="3" />
                    <label for="r3">3</label>
                  </div>
                  <!-- 4 -->
                  <div class="flex items-center gap-2.5">
                    <input id="r4" name="number-room" type="radio" value="4" />
                    <label for="r4">4</label>
                  </div>
                </div>
              </div>

              <!--        range  input   item         -->
              <div class="repair__calculate-form-item range">
                <h2 class="title">Площадь, м2:</h2>
                <!--                inputs wrapper       -->
                <div class="grid grid-cols-1 w-full">
                  <!-- 1 -->
                  <div class="flex items-center gap-x-4">
                    <input
                      id="ra1"
                      type="range"
                      :min="0"
                      :max="200"
                      :step="1"
                      v-model="repair_range"
                    />
                    <label for="ra1">{{ repair_range }}</label>
                  </div>
                  <!--  -->
                </div>
              </div>
            </div>

            <div class="repair__calculate-discount-wrap">
              <div class="repair__calculate-discount">
                <div>
                  <p>Срок ремонта:</p>
                  <h2>до 34 дней</h2>
                </div>
                <div>
                  <p>Скидка составит:</p>
                  <h2>23 765 руб</h2>
                </div>
              </div>
            </div>

            <div class="repair__calculate-enter-phone">
              <h2 class="title">Введите номер телефона</h2>

              <div class="inputs">
                <input type="number" placeholder="+7" />
                <button type="submit">Заказать</button>
              </div>
            </div>
          </form>
        </div>
      </div>
    </div>

    <!--      Repair prices cards is wrapper      -->
    <div class="repair__prices">
      <div class="container">
        <div class="repair__prices-title">
          <h2>Цены на ремонт</h2>
        </div>

        <div class="repair__prices-wrapper">
          <!-- card.s -->
          <repairPricesCard v-for="i in 5" :key="i" />
        </div>
      </div>
    </div>

    <!--       Examples of our work          -->
    <div class="example__works">
      <div class="container">
        <h2 class="example__works-title">Примеры наших работ</h2>
      </div>
    </div>
    <!-- qoldirildi -->

    <!-- Stock section -->
    <div class="stock">
      <div class="container">
        <h2 class="stock-title">Акции</h2>

        <div class="stock-card-wrapper">
          <div class="stock-card" v-for="i in 3" :key="i">
            <div class="stock-card-img">
              <img
                src="~assets\images\stock_images\stock-card-img.png"
                alt=""
              />
            </div>
            <div class="stock-card-info">
              <h2>Новоселам</h2>
              <p>Специальная скидка для тех кто переехал не более года назад</p>
            </div>
            <div class="stock-card-btn">
              <button>Получить скидку</button>
            </div>
          </div>
        </div>

        <div class="stock-all">
          <button>Все акции</button>
        </div>
      </div>
    </div>

    <!--    we work section -->
    <div class="we__work">
      <div class="container">
        <h2 class="we__work-title">Как мы работаем</h2>
        <p class="we__work-sub-title">
          Вам понятен каждый этап: фиксированные сроки и цены, предоставляем все
          документы: накладные, гарантии, акты. Вы будете уверены в результате.
        </p>
      </div>
    </div>
    <!--  qoldirildi   -->

    <!-- partners -->
    <div class="partners">
      <div class="container">
        <h2 class="partners-title">
          Свой склад и шоурум материалов наших партнеров в Москве
        </h2>

        <ul class="partners-services">
          <!-- 1 -->
          <li class="partners-services-item">
            <div class="img">
              <img src="~assets\images\partners\partners-1.svg" alt="img" />
            </div>
            <div class="info">
              <p>Прямой договор с поставщиками</p>
            </div>
          </li>
          <!-- 2 -->
          <li class="partners-services-item">
            <div class="img">
              <img src="~assets\images\partners\partners-2.svg" alt="img" />
            </div>
            <div class="info">
              <p>Доставка и подьём в квартиру</p>
            </div>
          </li>
          <!-- 3 -->
          <li class="partners-services-item">
            <div class="img">
              <img src="~assets\images\partners\partners-3.svg" alt="img" />
            </div>
            <div class="info">
              <p>300 тонн черновых и чистовых материалов</p>
            </div>
          </li>
          <!-- 4 -->
          <li class="partners-services-item">
            <div class="img">
              <img src="~assets\images\partners\partners-4.svg" alt="img" />
            </div>
            <div class="info">
              <p>250 видов обоев</p>
              <p>25 видов ламината</p>
              <p>50 видов плитки и плинтуса</p>
            </div>
          </li>
          <!-- 5 -->
          <li class="partners-services-item">
            <div class="img">
              <img src="~assets\images\partners\partners-5.svg" alt="img" />
            </div>
            <div class="info">
              <p>Выезд специалиста с каталогом материалов</p>
            </div>
          </li>
        </ul>

        <ul class="partners-textures">
          <li>
            <img src="~assets\images\partners\textture-1.png" alt="img" />
          </li>
          <li>
            <img src="~assets\images\partners\textture-2.png" alt="img" />
          </li>
        </ul>
      </div>
    </div>

    <!-- quality control -->
    <div class="quality__control">
      <div class="container">
        <h2 class="quality__control-title">Многоуровневый контроль качества</h2>
        <p class="quality__control-sub-title">
          Ремонтируем квартиры без дефектов благодаря многоуровневому контролю
          качества:
        </p>
      </div>
      <div class="quality__control-wrapper">
        <div class="quality__control-wrapper-img">
          <img
            src="~assets\images\png\quality__control-wrapper-img.png"
            alt="quality__control-wrapper-img"
          />
        </div>

        <ul class="quality__control-wrapper-items">
          <!-- 1 -->
          <li class="quality__control-wrapper-item">
            <div class="number">
              <h2>01</h2>
              <span>/05</span>
            </div>
            <h2 class="title">Главный инженер</h2>
            <p class="desc">
              Наблюдает за работой в режиме реального времени. Проверяет
              поставщиков материалов и оборудования
            </p>
          </li>
          <!-- 2 -->
          <li class="quality__control-wrapper-item">
            <div class="number">
              <h2>02</h2>
              <span>/05</span>
            </div>
            <h2 class="title">Отдел технического конроля</h2>
            <p class="desc" style="margin-top: 11px">
              Проверяет качество работ на всех объектах-решает спорные ситуации
            </p>
          </li>
          <!-- 3 -->
          <li class="quality__control-wrapper-item">
            <div class="number">
              <h2>03</h2>
              <span>/05</span>
            </div>
            <h2 class="title">Видео и фото контроль</h2>
            <p class="desc">Онлайн-контроль хода ремонта 24/7</p>
          </li>
          <!-- 4 -->
          <li class="quality__control-wrapper-item">
            <div class="number">
              <h2>04</h2>
              <span>/05</span>
            </div>
            <h2 class="title">Начальник участка</h2>
            <p class="desc">
              Оценивает соответствие процесса ремонта условиям договора по
              срокам и стоимости.
            </p>
          </li>
          <!-- 5 -->
          <li class="quality__control-wrapper-item">
            <div class="number">
              <h2>05</h2>
              <span>/05</span>
            </div>
            <h2 class="title">Прораб</h2>
            <p class="desc">
              Приезжает на объект 4-5 раз в неделю, контролирует работу
              мастеров. Проверяет каждый этап по 120 пунктам соответсвия.
            </p>
          </li>
        </ul>
      </div>
    </div>

    <!-- Our advantages -->
    <div class="our__advantages">
      <div class="container">
        <h2 class="our__advantages-title">Наши преимущества</h2>

        <ul class="our__advantages-wrapper">
          <!-- 1 -->
          <li class="our__advantages-wrapper-item">
            <div class="img">
              <img
                src="~\assets\images\our__advantages\our__advantages-1.svg"
                alt="img"
              />
            </div>
            <h2 class="title">Работа без предоплаты</h2>
            <p class="desc">
              Мы не берём предоплату. Вы платите за каждый этап работ после
              подписания акта.
            </p>
          </li>
          <!-- 2 -->
          <li class="our__advantages-wrapper-item">
            <div class="img">
              <img
                src="~\assets\images\our__advantages\our__advantages-2.svg"
                alt="img"
              />
            </div>
            <h2 class="title">Стоимость ремонта не меняется</h2>
            <p class="desc">
              Прозрачный бюджет. Финальная смета фиксируется в согласованных
              актах.
            </p>
          </li>
          <!-- 3 -->
          <li class="our__advantages-wrapper-item">
            <div class="img">
              <img
                src="~\assets\images\our__advantages\our__advantages-3.svg"
                alt="img"
              />
            </div>
            <h2 class="title">Мастера-славяне с опытом от 5 лет</h2>
            <p class="desc">
              Мастера - славяне. В штате 250 мастеров с опытом работы от 5 лет,
              20 прорабов с опытом от 8 лет и инженерным образованием.
            </p>
          </li>
          <!-- 4 -->
          <li class="our__advantages-wrapper-item">
            <div class="img">
              <img
                src="~\assets\images\our__advantages\our__advantages-4.svg"
                alt="img"
              />
            </div>
            <h2 class="title">За нами не переделывают</h2>
            <p class="desc">
              Качество работ для нас в приоритете. Даём гарантию на все виды
              работ.
            </p>
          </li>
        </ul>
      </div>
    </div>

    <!-- Reviews -->
     <div class="reviews">
      <div class="container">
        <h2 class="reviews-title">Отзывы</h2>
      </div>
     </div>
  </div>
</template>

<script setup>
// import's
import repairPricesCard from "~/component/repairPricesCard.vue";
// varibles
const repair_range = ref(35);
</script>

<style lang="scss" scoped></style>
