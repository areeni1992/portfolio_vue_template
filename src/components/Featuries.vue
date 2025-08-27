<template>
  <div class="featuries container mx-auto">
    <div class="grid grid-cols-1 lg:grid-cols-2 gap-4 mx-10">
      <div class="content order-2 lg:order-1">
        <h2 class="text-orange-400 tracking-widest">FEATRIES</h2>
        <p class="text-4xl lg:text-7xl text-orange-950 font-bold">
          Give Your Site A New Look
        </p>
        <p>
          Service range including technical skills, design, business
          understanding.
        </p>
        <ul class="list-inside mt-10 space-y-4">
          <li>
            <span>
              <img
                src="@/assets/icons/featuries-check.png"
                alt="check"
                class="inline w-5 h-5 mr-2"
              />
              Clean Code</span
            >
          </li>
          <li>
            <span>
              <img
                src="@/assets/icons/featuries-check.png"
                alt="check"
                class="inline w-5 h-5 mr-2"
              />
              Modern Design</span
            >
          </li>
          <li>
            <span>
              <img
                src="@/assets/icons/featuries-check.png"
                alt="check"
                class="inline w-5 h-5 mr-2"
              />
              Responsive Layout</span
            >
          </li>
        </ul>
      </div>
      <div class="media relative w-full h-full order-1 lg:order-1">
        <span
          class="image before:bg-[url(@/assets/icons/featuries-back.png)] before:absolute before:w-70 before:h-70 lg:before:w-[470px] lg:before:h-[319px] before:bg-contain before:bg-no-repeat before:top-0 before:left-[15%] lg:before:top-[-15px] lg:before:left-30"
        >
          <img
            src="@/assets/icons/featuries-front.png"
            alt="front"
            class="lg:mt-30 lg:ml-40 relative z-1 w-70 lg:w-fit lg:h-[300px]"
          />
          <span
            class="arrow before:absolute before:bg-[url(@/assets/icons/featuries-man.png)] before:bg-size-[100px] lg:before:bg-auto before:bg-no-repeat before:top-0 before:left-0 lg:before:top-0 lg:before:left-50 before:w-40 before:h-40 lg:before:w-50 lg:before:h-50 before:z-10"
          ></span>
          <span
            class="arrow before:absolute before:bg-[url(@/assets/icons/featuries-arrow.png)] before:bg-no-repeat before:bg-size-[90px] before:top-[-20px] before:left-50 lg:before:top-[-30px] lg:before:right-[-390px] w-20 h-10 before:w-30 before:h-50"
          ></span>
          <span
            class="arrow before:absolute before:bg-[url(@/assets/icons/featuries-yellow.png)] before:bg-size-[200px] lg:before:bg-auto before:bg-no-repeat bottom-0 before:bottom-[-90px] before:right-10 lg:before:bottom-[-50px] before:w-[200px] before:h-[200px] lg:before:w-[370px] lg:before:h-[280px]"
          ></span>
          <span
            class="arrow before:absolute before:bg-[url(@/assets/icons/featuries-cloud.png)] before:bg-size-[20px] lg:before:bg-auto before:bg-no-repeat before:bottom-[0px] before:left-10 lg:before:bottom-[-120px] lg:before:left-15 before:w-50 before:h-50"
          ></span>
        </span>
      </div>
    </div>
  </div>
</template>
