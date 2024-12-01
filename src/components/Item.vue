<script setup></script>

<template>
  <div class="mx-1 mb-1 bg-white cursor-default shadow-black hover:scale-105 hover:shadow-xl transition-transform">
    <img
      src="/images/uno-p.jpg"
      alt="image"
      class="object-cover aspect-square"
    />
    <div class="p-2">
      <p class="text-center font-light">Arduino Uno</p>
      <div class="flex justify-between items-baseline">
        <p class="line-through text-gray-500 text-sm font-light">₱ 500.00</p>
        <p class="text-lg text-orange-500 font-semibold">₱ 498.00</p>
      </div>
    </div>
    <div>
      <button
        class="w-full py-1.5 text-center text-white bg-gradient-to-r from-rose-500 to-orange-500"
      >
        Add to Cart
      </button>
    </div>
  </div>
</template>
