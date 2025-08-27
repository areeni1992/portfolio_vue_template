<template>
  <div class="sm:hidden md:block bg-gray-800 text-white w-full">
    <header class="container mx-auto flex items-center justify-between p-4">
      <span>
        <router-link to="/">
          <img src="@/assets/logo.png" alt="Logo" class="h-10" />
        </router-link>
      </span>
      <nav class="mx-auto flex space-x-4">
        <router-link to="/" class="px-4 py-2 hover:bg-gray-700"
          >Home</router-link
        >
        <router-link to="/about" class="px-4 py-2 hover:bg-gray-700"
          >About</router-link
        >
        <router-link to="/services" class="px-4 py-2 hover:bg-gray-700"
          >Services</router-link
        >
        <router-link to="/pricing" class="px-4 py-2 hover:bg-gray-700"
          >Pricing</router-link
        >
        <router-link to="/blog" class="px-4 py-2 hover:bg-gray-700"
          >Blog</router-link
        >
      </nav>
      <button
        class="border border-gray-400 px-5 py-2 rounded hover:bg-amber-600 hover:border-amber-600 cursor-pointer"
      >
        CONTACT
      </button>
    </header>
  </div>
</template>
