<template>
  <div class="max-w-[1558px] m-xl:mx-20  mx-auto my-28  flex items-center gap-6">
    <div class="w-full h-[300px] m-xl:h-[240px] rounded-[10px] bg-[#F5F5F5] flex justify-between">
      <div class="flex flex-col justify-center gap-8 m-xl:gap-3 px-14">
        <h4 class="font-black text-4xl xl:text-2xl">
          فروش ویژه <span class="text-[#1146C8]">کنسول گیمینگ</span> و محصولات <span class="text-[#EC641E]">اپل</span>
        </h4>
        <p class="text-xl  xl:text-base text-[#747474]">
          لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم
        </p>
        <button
          class="flex items-center justify-center gap-2 rounded-[40px] w-32 m-xl:w-24 h-12 m-xl:h-10 m-xl:text-sm font-bold text-xl text-white bg-gradient-to-tr from-[#76D2FF] to-[#0181C4]"
        >
          <span>مشاهده</span>
          <NuxtIcon name="main/black-arrow-left" />
        </button>
      </div>
      <nuxt-img
        src="/images/main/iphone.png"
        height="full"
        width="full"
        class="mx-8 my-5"
      />
    </div>
    <div
      class="w-full h-[300px] m-xl:h-[240px] rounded-[10px] left-box flex items-center justify-between overflow-hidden"
    >
      <div class="flex flex-col justify-center gap-8  m-xl:gap-3 px-14">
        <h4 class="font-black text-4xl m-xl:text-2xl ">هندزفری بیسیم <span class="m-xl:text-3xl text-[#0181C4]">شـــــــارک</span></h4>
        <p class="text-xl xl:text-base text-[#1E1E1E]">
          لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ
        </p>
        <button
          class="flex items-center justify-center gap-2 rounded-[40px] w-32 m-xl:w-24 h-12 m-xl:h-10 m-xl:text-sm font-bold text-xl text-white bg-gradient-to-tr from-[#76D2FF] to-[#0181C4]"
        >
          <span>مشاهده</span>
          <NuxtIcon name="main/black-arrow-left" />
        </button>
      </div>
      <div class="h-full aspect-square">
        <nuxt-img src="/images/main/headphone.png" fit="fill"  class="" />
      </div>
    </div>
  </div>
</template>

<script setup lang="ts"></script>

<style scoped>
.left-box {
  background: linear-gradient(
    180deg,
    #e3f4fe 0%,
    #e1f3ff 33.22%,
    #e3f4fe 59.8%,
    #eaf4fe 100%
  );
}
</style>
