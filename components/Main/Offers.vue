<template>
  <div
    class="max-w-[1558px] m-xl:mx-20 mx-auto my-20 px-6 h-[454px] m-xl:h-[410px] bg-gray-b8 rounded-2xl flex items-center justify-between"
  >
    <div class="w-[350px] m-xl:w-[310px] mx-auto">
      <div class="gift-cart w-44 mx-auto relative z-20">
        <p class="font-black text-3xl text-primary-b4 leading-[50px]">
          پیشنهادهای شگفت انگیز
          <span class="text-primary-orginal">آسان مارکت</span>
        </p>
        <nuxt-img src="images/main/gift.png" />
      </div>
    </div>

    <swiper
      :space-between="24"
      :breakpoints="{
        1600: {
          slidesPerView: 4,
        },
      }"
      class="cart-box overflow-x-hidden flex justify-between gap-6 px-6 rounded-xl w-full select-none"
      :modules="[Autoplay]"
      :autoplay="{ delay: 2000}"
      :slides-per-view="3"
      :navigation="{ nextEl: '.next-el-new', prevEl: '.prev-el-new' }"
    >
      <swiper-slide v-for="card in newProducts" :key="card.id">
        <UtilsCard
          :image="card.image"
          :category="card.category"
          :description="card.description"
          :rate="card.rate"
          :price="card.price"
          :liked="card.liked"
          @like-handler="card.liked = !card.liked"
        />
      </swiper-slide>
    </swiper>
  </div>
</template>

<script setup lang="ts">
import { SwiperSlide, Swiper } from "swiper/vue";
import { Autoplay } from "swiper";
const newProducts = ref([
  {
    id: 1,
    image: "images/products/memory1.png",
    category: "ذخیره سازی",
    description: "فلش مموری سامسونگ M20k11gh 16GB",
    rate: 2,
    price: "824,000",
    liked: false,
  },
  {
    id: 2,
    image: "images/products/watch.png",
    category: "ذخیره سازی",
    description: "ساعت هوشمند طرح اپل مدل NG4521",
    rate: 4,
    price: "547,000",
    liked: true,
  },
  {
    id: 3,
    image: "images/products/memory2.png",
    category: "ذخیره سازی",
    description: "بلوتوث فندکی سفید برند وریتی",
    rate: 1,
    price: "908,000",
    liked: false,
  },
  {
    id: 4,
    image: "images/products/watch.png",
    category: "ذخیره سازی",
    description: "ساعت هوشمند طرح اپل مدل NG4521",
    rate: 5,
    price: "824,000",
    liked: false,
  },
  {
    id: 5,
    image: "images/products/memory2.png",
    category: "ذخیره سازی",
    description: "بلوتوث فندکی سفید برند وریتی",
    rate: 1,
    price: "908,000",
    liked: false,
  },
  {
    id: 6,
    image: "images/products/memory2.png",
    category: "ذخیره سازی",
    description: "بلوتوث فندکی سفید برند وریتی",
    rate: 1,
    price: "908,000",
    liked: false,
  },
  {
    id: 7,
    image: "images/products/watch.png",
    category: "ذخیره سازی",
    description: "ساعت هوشمند طرح اپل مدل NG4521",
    rate: 5,
    price: "824,000",
    liked: false,
  },
  {
    id: 8,
    image: "images/products/memory2.png",
    category: "ذخیره سازی",
    description: "بلوتوث فندکی سفید برند وریتی",
    rate: 1,
    price: "908,000",
    liked: false,
  },
]);
</script>

<style scoped>
.cart-box {
  box-shadow: -25px 0px 23px -15px #00000040, 25px 0px 23px -15px #00000040;
}
.gift-cart {
  z-index: 10;
}
</style>
