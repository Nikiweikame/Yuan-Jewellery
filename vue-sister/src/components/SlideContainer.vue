<script setup>
import { ref } from "vue";
import Slide from "../components/Slide.vue";

const sildeDataArray = ref([
  {
    title: "苑・飾物",
    subTitle: "所有作品與你們與自然相互依存，畫一個和諧的圓。",
    button: "主打商品",
    background: "/First.jpg",
    indexID: "rs-3045",
    path: "#product",
  },
  {
    title: "苑・飾物",
    subTitle:
      "每個首飾都發想於NI生活周遭的人、事、物，用首飾紀錄生活上的感受與體悟。",
    button: "IG動態",
    background: "/image 9.png",
    indexID: "rs-30451",
    path: "#IG",
  },
  {
    title: "近期活動",
    subTitle: "海玻璃Ｘ簡易金繼 手作飾品工作坊",
    button: "詳細介紹",
    background: "/活動.png",
    indexID: "rs-30452",
    path: "#lastest",
  },
]);
</script>
<template>
  <div class="example">
    <div class="content">
      <div
        id="rev_slider_1078_1_wrapper"
        class="rev_slider_wrapper fullwidthbanner-container"
        data-alias="classic4export"
        data-source="gallery"
        style="
          margin: 0px auto;
          background-color: transparent;
          padding: 0px;
          margin-top: 0px;
          margin-bottom: 0px;
        "
      >
        <!-- START REVOLUTION SLIDER 5.4.1 fullwidth mode -->
        <div
          id="rev_slider_1078_1"
          class="rev_slider fullwidthabanner"
          data-version="5.4.1"
        >
          <!-- SLIDE  -->
          <ul>
            <Slide v-for="SildeDate in sildeDataArray" :slideDate="SildeDate" />
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
.content {
  padding-top: 0;
  padding-bottom: 0;
}
@media (min-width: 1024px) {
}
</style>
