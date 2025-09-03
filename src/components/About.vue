<template>
  <div class="about container mx-auto py-15">
    <div class="grid grid-cols-1 lg:grid-cols-2 gap-4">
      <div class="media">
        <span
          class="image relative before:bg-[url(@/assets/icons/about-back.png)] before:absolute before:w-70 before:h-70 lg:before:w-[470px] lg:before:h-[319px] before:bg-contain before:bg-no-repeat before:top-0 before:left-[15%] lg:before:top-[-15px] lg:before:left-30"
        >
          <img
            src="@/assets/icons/about-front.png"
            alt="front"
            class="mt-20 ml-20 lg:mt-30 lg:ml-40 relative z-1 w-70 lg:w-fit lg:h-[300px]"
          />
          <span
            class="arrow before:absolute before:bg-[url(@/assets/icons/about-cloud.png)] before:bg-no-repeat before:top-0 before:left-0 lg:before:top-10 lg:before:left-20 w-20 h-10 before:w-full before:h-full"
          ></span>
          <span
            class="arrow before:absolute before:bg-[url(@/assets/icons/about-arrow.png)] before:bg-no-repeat before:bg-size-[90px] before:top-[-20px] before:left-50 lg:before:top-[-30px] lg:before:right-[-390px] w-20 h-10 before:w-30 before:h-50"
          ></span>
          <span
            class="arrow before:absolute before:bg-[url(@/assets/icons/about-colors.png)] before:bg-size-[200px] lg:before:bg-auto before:bg-no-repeat before:top-0 lg:before:top-0 before:right-0 lg:before:right-[-330px] w-10 h-10 before:w-50 before:h-[80px] lg:before:w-full lg:before:h-full"
          ></span>
          <span
            class="arrow before:absolute before:bg-[url(@/assets/icons/about-man.png)] before:bg-size-[120px] lg:before:bg-auto before:bg-no-repeat before:bottom-[-140px] before:left-10 lg:before:bottom-[-320px] lg:before:left-15 before:w-50 before:h-50 lg:before:w-full lg:before:h-full before:z-10"
          ></span>
        </span>
      </div>
      <div class="content space-y-20 pl-10 mt-20 lg:pl-0 lg:mt-0 lg:space-y-5">
        <h1 class="text-orange-500 tracking-widest">ABOUT</h1>
        <p class="text-4xl lg:text-5xl font-bold text-amber-950">
          An Experience <br />
          Design Agency
        </p>
        <p class="text-amber-950 font-semibold">
          Provides a full service range
        </p>
        <p class="text-amber-900 text-lg">
          Ability to put themselves in the merchant's shoes.<br />
          It is meant to partner on the long run, and work as an extension
          <br />
          of the merchant's team.
        </p>
        <button
          class="bg-white py-3 px-6 rounded shadow relative z-10 hover:bg-amber-500 hover:text-white transition mt-6 cursor-pointer"
        >
          About Us
        </button>
      </div>
    </div>
    <div class="counter mx-10 lg:mx-auto my-20 lg:mt-70">
      <div class="flex flex-col lg:grid lg:grid-cols-3 gap-4 lg:gap-10 mt-10 lg:mt-0 border-1 border-orange-200 rounded h-40 lg:h-40">
        <div class="flex flex-col items-center justify-center">
          <p class="text-4xl font-bold text-amber-950">42%</p>
          <span class="text-amber-900">Years of experience</span>
        </div>
        <div class="flex flex-col items-center justify-center border-l-1 border-r-1 border-orange-200 px-10">
          <p class="text-4xl font-bold text-amber-950">73+</p>
          <span class="text-amber-900">Agency members</span>
        </div>
        <div class="flex flex-col items-center justify-center">
          <p class="text-4xl font-bold text-amber-950">5.000</p>
          <span class="text-amber-900">Projects complete</span>
        </div>
      </div>
    </div>
  </div>
</template>
