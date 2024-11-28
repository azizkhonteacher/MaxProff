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
          <repairPricesCard v-for="i in 5" :key="i"/>
        </div>
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
