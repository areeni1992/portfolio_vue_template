<script setup>
import laptopBackground from "@/assets/icons/laptop_background.png";
import Oval from "@/assets/icons/Oval.png";
import girlImage from "@/assets/icons/girl_image.png";
</script>
<template>
  <div
    class="hero container grid grid-cols-1 lg:grid-cols-2 gap-6 mx-auto py-15 "
  >
    <div class="content space-y-4 p-5 order-1 md:order-0">
      <div class="title text-amber-700 uppercase">Modern Studio</div>
      <p class="text-6xl text-white font-bold">
        We’re Help To Build Your Dream Project
      </p>
      <p class="text-sm text-gray-400 my-8 sm:text-lg">
        Agency provides a full service range including technical skills,<br />design,
        business understanding.
      </p>
      <div
        class="btnsflex flex-col sm:flex-row justify-center lg:justify-start gap-4 mt-6 space-x-1.5"
      >
        <button
          class="bg-amber-600 text-white py-3 px-6 rounded hover:bg-amber-700 transition"
        >
          HOW WE WORK
        </button>
        <button
          class="text-white py-3 px-6 rounded hover:bg-white hover:text-black transition"
        >
          Contact Us
        </button>
      </div>
    </div>
    <div
      class="shaps relative w-full h-[400px] sm:h-[500px] md:h-[600px] inset-0 sm:bg-size-[60%] lg:bg-size-contain"
    >
      <div
        class="absolute bg-contain bg-no-repeat ml-5 w-[130px] h-[150px] lg:w-70 lg:h-full left-0 top-0 text-center z-10"
        :style="{ backgroundImage: `url(${laptopBackground})` }"
      >
          <img
            src="@/assets/icons/laptop.png"
            alt=""
            class="top-[50px] left-10 ml-5 mt-7 h-fit"
          />
      </div>
      <div
        class="absolute bg-contain bg-no-repeat left-50 top-[-50] lg:left-90 lg:top-10 w-[80px] h-[80px] lg:h-30 lg:w-30 flex justify-center items-center"
        :style="{ backgroundImage: `url(${Oval})` }"
      >
        <img src="@/assets/icons/stars.png" alt="" class="w-10" />
      </div>
      <div
        class="absolute z-20 bg-contain bg-no-repeat right-0 top-[90px] lg:top-30 lg:w-30 lg:h-20"
      >
        <img src="@/assets/icons/wave_shap.png" alt="" class="w-fit" />
      </div>
      <div
        class="absolute left-10 z-40 bottom-[-50px] bg-contain bg-no-repeat before:bg-[url(@/assets/icons/curve_arrow.png)] before:absolute before:w-20 before:h-20 lg:before:w-50 lg:before:h-20 before:bg-contain before:bg-no-repeat before:top-[-150px] before:left-[0px] lg:before:top-[-90px] lg:before:left-[-30px]"
      >
        <img src="@/assets/icons/id.png" alt="" class="w-40 lg:w-fit relative top-[-90px] left-[-30px] lg:static lg:left-none lg:top-auto" />
      </div>
      <div
        class="absolute bg-contain z-10 bg-no-repeat right-10 bottom-[-90px] w-35 h-70 lg:w-50 lg:h-80 before:absolute before:bg-[url(@/assets/icons/curve-2_arrow.png)] before:w-30 before:h-50 before:bg-contain before:bg-no-repeat before:bottom-[-80px] before:left-[-50px] lg:before:bottom-[-200px] lg:before:left-[-150px]"
        :style="{ backgroundImage: `url(${girlImage})` }"
      ></div>
    </div>
  </div>
  <div
    class="testimonials container mx-auto flex space-x-1.5 py-15 bg-gray-800"
  >
    <img src="@/assets/icons/man_image.png" alt="man" />
    <div class="max-w-7xl text-white">
      <p class="text-gray-400">"Put themselves in the merchant's shoes"</p>
      <span>Meta Inc.</span>
    </div>
  </div>
</template>
<style scoped>
.shaps {
  background-image: url("@/assets/icons/circle.png");
  background-repeat: no-repeat;
  background-position: center;
}
</style>
