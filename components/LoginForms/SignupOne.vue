<template>
  <div class="w-full flex flex-col justify-center h-full">
    <h3 class="font-semibold text-2xl mb-10 text-[#CCCCCC]">
      شماره همراه خود را وارد نمایید
    </h3>

    <form class="w-[434px]">
      <div class="input-wrapper" dir="ltr">
        <label class="input-label" for="username">شماره همراه</label>
        <input type="text" name="username" id="username" class="input-field" />
      </div>

      <!-- ------------------- BUTTONS -------------------- -->
      <div class="mt-14 flex items-center w-full gap-4">
        <button @click.prevent="handleChange" class="w-full c-btn-primary">
          دریافت کد
        </button>
      </div>
    </form>
  </div>
</template>

<script setup lang="ts">
const emit = defineEmits(["change-page"]);

const handleChange = () => {
  emit("change-page", 2);
};
</script>

<style scoped></style>
