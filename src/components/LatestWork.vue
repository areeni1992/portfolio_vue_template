<script setup>
import { ref, computed } from "vue";
import portraitImg from "@/assets/icons/latestwork.png";
import portraitImg2 from "@/assets/icons/latestwork-2.png";
import portraitImg3 from "@/assets/icons/latestwork-3.png";
import portraitImg4 from "@/assets/icons/latestwork-4.png";
// State
const selectedCategory = ref("All");
const showAll = ref(false);
// Data
const categories = [
  {
    name: "All",
    count: 4,
    subcategories: ["Branding", "Design", "Photography", "Development"],
  },
  {
    name: "Branding",
    count: 8,
    products: [
      { name: "Icon", image: portraitImg },
      { name: "Templates", image: portraitImg2 },
      { name: "Logo", image: portraitImg3 },
      { name: "Mockup", image: portraitImg4 },
    ],
  },
  {
    name: "Design",
    count: 12,
    products: [
      { name: "UI Kit", image: portraitImg },
      { name: "Wireframe", image: portraitImg2 },
      { name: "Landing Page", image: portraitImg3 },
      { name: "Dashboard", image: portraitImg4 },
    ],
  },
  {
    name: "Photography",
    count: 4,
    products: [
      { name: "Portrait", image: portraitImg },
      { name: "Landscape", image: portraitImg2 },
      { name: "Studio", image: portraitImg3 },
      { name: "Event", image: portraitImg4 },
    ],
  },
  {
    name: "Development",
    count: 6,
    products: [
      { name: "Vue App", image: portraitImg },
      { name: "Laravel API", image: portraitImg2 },
      { name: "SSR Site", image: portraitImg3 },
      { name: "Tailwind UI", image: portraitImg4 },
    ],
  },
];

// Show All Products

// Computed filter
const filteredProducts = computed(() => {
  if (selectedCategory.value === "All") {
    return categories.flatMap(
      (cat) =>
        cat.products?.map((prod) => ({
          ...prod,
          category: cat.name,
        })) || []
    );
  } else {
    const category = categories.find(
      (cat) => cat.name === selectedCategory.value
    );
    return (
      category?.products?.map((prod) => ({
        ...prod,
        category: category.name,
      })) || []
    );
  }
});

const visibleItems = computed(() => {
  return showAll.value ? filteredProducts : filteredProducts.slice(0, 4);
});
</script>

<template>
  <div class="title text-center mt-20">
    <h3 class="text-orange-400 tracking-widest">Portofolio</h3>
    <h2 class="text-7xl text-white font-bold">Latest Work</h2>
  </div>
  <div class="categories flex flex-wrap justify-center space-x-4 my-20">
    <button
      v-for="category in categories"
      :key="category.name"
      @click="selectedCategory = category.name"
      :class="[
        selectedCategory === category.name
          ? 'text-white font-semibold'
          : 'text-gray-400',
      ]"
      class="relative px-4 py-2 rounded text-gray-400 hover:text-orange-100 cursor-pointer"
    >
      <span></span>
      <span class="text-gray-400 absolute top-0 right-0">
        {{ category.count }}
      </span>
      {{ category.name }}
    </button>
  </div>
  <transition-group
    name="fade"
    tag="div"
    class="container mx-auto px-10 grid grid-cols-1 lg:grid-cols-5 gap-6 mt-10"
  >
    <div
      v-for="(product, index) in filteredProducts.slice(0, 4)"
      :key="product.name"
      class="relative overflow-hidden shadow hover:scale-101 transition lg:nth-[2n+1]:col-span-2 lg:nth-[1n+2]:col-span-3"
    >
      <img
        :src="product.image"
        :alt="product.name"
        class="w-full h-95 object-cover mb-2 rounded"
        :style="{ animationDelay: `${index * 100}ms` }"
      />
      <h2 class="absolute bottom-20 left-5 bg-white rounded-3xl px-3 py-2">
        {{ product.category }}
      </h2>
      <h3 class="text-4xl absolute bottom-5 left-5 text-white font-semibold">
        {{ product.name }}
      </h3>
    </div>
  </transition-group>
  <button
    class="mx-auto py-2 px-10 rounded border border-white text-white font-bold"
    v-if="!showAll"
    @click="visibleItems"
  >
    Show More
  </button>
</template>

<style scoped>
/* Fade + Scale + Staggered Motion */
.fade-enter-active {
  animation: fadeIn 0.5s ease forwards;
  overflow: hidden;
}

.fade-leave-active {
  animation: fadeOut 0.4s ease forwards;
  position: absolute;
  width: 100%;
}

/* Initial states */
.fade-enter-from {
  opacity: 0;
  transform: scale(0.95) translateY(20px);
}

.fade-leave-to {
  opacity: 0;
  transform: scale(0.95) translateY(-20px);
}

/* Keyframes for smoother control */
@keyframes fadeIn {
  0% {
    opacity: 0;
    transform: scale(0.95) translateY(20px);
  }
  100% {
    opacity: 1;
    transform: scale(1) translateY(0);
  }
}

@keyframes fadeOut {
  0% {
    opacity: 1;
    transform: scale(1) translateY(0);
  }
  100% {
    opacity: 0;
    transform: scale(0.95) translateY(-20px);
  }
}
</style>
