<style scoped lang="scss">
.lastest-activty {
  padding: 60px 16px;
  &__title {
    font-family: "Noto Sans TC", sans-serif;
    text-align: center;
    font-size: 24px;
  }
  .card {
    text-decoration: none;
    border: 0;
  }
  .card-body {
    padding: 16px 0;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    height: 200px;
  }
  .card-title {
    white-space: nowrap;
  }
  .card-text {
    margin: 0;
    &:last-child {
      text-align: end;
    }
  }
  .text-body-secondary {
    padding: 0 16px;
    white-space: nowrap;
  }
}
@media screen and (min-width: 992px) {
  .lastest-activty {
    padding: 60px;
  }
}
@media screen and (min-width: 1200px) {
  .lastest-activty {
    .card-body {
      padding: 0 0 0 16px;
      height: 100%;
    }
  }
}
</style>

<script setup>
import { ref } from "vue";
const activityArray = ref([
  {
    link: "https://www.accupass.com/event/2304211356524296756490",
    image: "./src/assets/lastest-activity_01.jpeg",
    title: "海玻璃Ｘ簡易金繼 手作飾品工作坊",
    content:
      "結合愛護環境、永續的理念，借鏡日本的「金繼」工藝簡化之後，運用在海玻璃上，製成獨一無二的飾品。不需要任何金工基礎，就能夠完成！一起來動動手吧！",
    date: "2023.05.20 (六) 14:00 - 17:00",
  },
  {
    link: "https://www.accupass.com/event/2305080421501006396929",
    image: "./src/assets/lastest-activity_02.jpeg",
    title: "簡易金繼海玻璃首飾工作坊",
    content:
      "【簡易金繼海玻璃首飾工作坊】跟著Yuan Jewellery，在川端藝會所，將散落在沙灘上的海玻璃，藉由簡易金繼變成一條條專屬於自己的海玻璃首飾吧！",
    date: "2023.06.03(六)14:00-16:00、06.07(三)19:30-21:30",
  },
]);
</script>
<template>
  <div class="lastest-activty" id="lastest">
    <p class="lastest-activty__title">近期活動</p>
    <div class="row">
      <div class="col-12 col-md-6" v-for="info in activityArray">
        <a :href="info.link" class="card">
          <div class="row g-0">
            <div class="col-md-12 col-xl-6">
              <img
                :src="info.image"
                class="img-fluid rounded-start"
                alt="..."
              />
            </div>
            <div class="col-md-12 col-xl-6">
              <div class="card-body">
                <h5 class="card-title">{{ info.title }}</h5>
                <p class="card-text">{{ info.content }}</p>
                <p class="card-text">
                  <small class="text-body-secondary">{{ info.date }}</small>
                </p>
              </div>
            </div>
          </div>
        </a>
      </div>
    </div>
  </div>
</template>
