<script setup>
import { Fancybox } from "@fancyapps/ui";
import "@fancyapps/ui/dist/fancybox/fancybox.css";
import { onMounted } from "vue";

onMounted(() => {
  Fancybox.bind("[data-fancybox]", {
    Toolbar: false, // hide toolbar
    defaultType: "iframe",
    iframe: {
      preload: false,
      css: {
        width: "100%",
        height: "100%",
        padding: "0",
      },
    },
  });
});
</script>

<template>
  <div class="video container mx-auto my-30 w-full">
    <div class="grid grid-cols-1 lg:grid-cols-2 lg:gap-8 mx-10 space-y-3 lg:space-y-0 lg:space-x-8">
      <div class="media relative">
        <a
          href="https://www.youtube.com/embed/PUdyuKaGQd4?autoplay=1"
          data-fancybox
          data-type="iframe"
          data-width="640"
          data-height="360"
        >
          <div class="overlay">
            <div class="play absolute flex items-center justify-center top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2">
              <img
                class="w-full h-full cursor-pointer"
                src="@/assets/icons/play.png"
                alt="Play Button"
              />
            </div>
            <img
              class="poster cursor-pointer"
              src="@/assets/icons/video_poster.png"
              alt="Video poster"
              width="100%"
              height="100%"
            />
          </div>
        </a>
      </div>
      <div class="content flex flex-col justify-center">
        <h3 class="text-orange-400 tracking-widest">VIDEO REEL</h3>
        <p class="text-4xl lg:text-5xl text-orange-950 font-bold">
          Unlock The Greatest Value Possible
        </p>
      </div>
    </div>
  </div>
</template>

<style scoped>
.overlay {
  position: relative;
}
.overlay::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
  width: 100%;
  height: 100%;
  border-radius: 7px;
  background: rgba(0, 0, 0, 0.3); /* Dark overlay */
}
</style>
