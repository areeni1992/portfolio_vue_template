<script setup>
import HeroSection from "@/components/HeroSection.vue";
import Projects from "@/components/Projects.vue";
import About from "@/components/About.vue";
import HowWeWork from "@/components/HowWeWork.vue";
import Video from "@/components/Video.vue";
import Featuries from "@/components/Featuries.vue";
import LatestWork from "@/components/LatestWork.vue";
</script>

<template>
  <main class="w-full">
    <div class="bg-gray-800">
      <HeroSection />
    </div>
    <div class="bg-[#FDF0E9]">
      <Projects />
      <About />
      <HowWeWork />
      <Video />
      <Featuries />
    </div>
    <div class="bg-gray-800 py-10">
      <LatestWork />
    </div>
  </main>
</template>
