<template>
  <div class="repair__prices-card">
    <div class="repair__prices-card-head">
      <div class="img">
        <img
          src="~/assets/images/png/hero_banner.png"
          alt="repair prices card img"
        />
      </div>

      <div class="title">
        <h2>Косметический</h2>
        <p>от 5 дней</p>
      </div>
    </div>
    <div class="repair__prices-card-desc">
      <p>
        Такой тип ремонта подойдёт для того чтобы «освежить» ремонт в квартире:
        заменить покрытие стен, пола и потолка без предварительной подготовки
      </p>
    </div>
    <span class="flex w-full" style="height: 2px; background: #2d4872"></span>

    <!-- shunga class qo'shiladi  class = dismantling-item-active-->
    <div class="repair__prices-card-dismantling">
      <div class="dismantling-item" v-for="i in 2" :key="i">
        <h2 class="dismantling-item-title">Демонтаж</h2>
        <ul class="dismantling-item-wrap">
          <li v-for="i in 3" :key="i">
            <checkSvg />
            <p>Демонтаж старых покрытий</p>
          </li>
        </ul>
      </div>
    </div>

    <div class="repair__prices-card-dismantling-more">
      <button @click="activeDismant($event)">
        Список работ <bottomArrowSvg />
      </button>
      <div class="price-wrap">
        <p class="old-price">от 3 245 руб/м2</p>
        <p class="new-price">от 2 450 руб/м2</p>
      </div>
    </div>

    <div class="repair__prices-card-GetAnEstimate">
      <button>Получить смету</button>
    </div>
  </div>
</template>

<script setup>
// import's
import checkSvg from "~/component/icon/checkSvg.vue";
import bottomArrowSvg from "~/component/icon/bottomArrowSvg.vue";
// function
function activeDismant(e) {
  // cardni tutib olamiz
  let target_parent = e.target.parentNode.parentNode;

  // class qo'shilishi kerak bo'lgan elementni tutamiz
  const dismantling = target_parent.querySelector(
    ".repair__prices-card-dismantling"
  );

  dismantling.classList.toggle("dismantling-item-active");
  console.log(dismantling);

  e.target.classList.toggle("dismantling-item-active-btn");
}
</script>

<style lang="scss" scoped></style>
