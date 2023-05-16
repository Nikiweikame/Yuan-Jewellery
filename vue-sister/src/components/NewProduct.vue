<template>
  <div class="new-product" id="product">
    <p class="new-product__title">主打商品</p>
    <div class="new-product__content">
      <div id="da-thumbs" class="da-thumbs portfolio row">
        <div
          class="pitem item-w1 item-h1 cat1 col-12 col-md-6 col-lg-3"
          v-for="(image, index) in product"
        >
          <a :href="image.link">
            <img
              class="new-product__img"
              :src="image.imgUrl"
              :alt="image.name"
            />
            <div class="">
              <span class="">{{ image.name }}</span>
            </div>
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
.new-product {
  padding: 60px 16px;
  &__img {
    width: 100%;
    height: 500px;
    object-fit: cover;
  }
  &__title {
    font-family: "Noto Sans TC", sans-serif;
    text-align: center;
    font-size: 24px;
  }
  .row {
    margin: 0;
  }
}

@media screen and (min-width: 992px) {
  .new-product {
    padding: 60px;
  &__img {
    height: 300px;
  }
  }
}
</style>

<script setup>
import { ref, onMounted, onUnmounted } from "vue";
const product = ref([
  {
    imgUrl: "https://cdn01.pinkoi.com/product/GWuTiPb6/0/1/800x0.jpg",
    name: "【客製化禮物】小小金海玻璃耳環(可改夾式)",
    link: "https://www.pinkoi.com/product/GWuTiPb6",
  },
  {
    imgUrl: "https://cdn01.pinkoi.com/product/ng5EujSR/0/1/800x0.jpg",
    name: "【客製化禮物】小小海玻璃戒指(開放式戒圍)",
    link: "https://www.pinkoi.com/product/ng5EujSR",
  },
  {
    imgUrl: "https://cdn01.pinkoi.com/product/akx9nLdi/0/1/800x0.jpg",
    name: "【客製化禮物】玻璃珍珠原碎純銀手鍊",
    link: "https://www.pinkoi.com/product/akx9nLdi",
  },
  {
    imgUrl: "https://cdn01.pinkoi.com/product/rkG5cikH/0/1/800x0.jpg",
    name: "【客製化禮物】玻璃原碎珍珠耳環",
    link: "https://www.pinkoi.com/product/rkG5cikH",
  },
]);
const script = document.createElement("script");
script.type = "text/javascript";
script.src = "./js/masonry.js";
// watch(counterStore.designSampleArray, () => {
//   document.body.appendChild(script);
// });
onMounted(() => {
  document.body.appendChild(script);
});
onUnmounted(() => {
  document.body.removeChild(script);
});
</script>
