<script setup></script>

<template>
  <div class="flex w-full justify-between items-center my-1 shadow-md shadow-gray-100 rounded-lg p-1 px-2">
    <div class="flex items-center">
      <input
        type="checkbox"
        name="check"
        class="accent-orange-500"
      />
      <img
        src="/images/uno-p.jpg"
        alt="uno"
        class="w-16 h-16 aspect-square object-cover ml-2"
      />
      <div class="ml-2">
        <p class="font-light">Arduino Uno</p>
        <p class="text-sm text-orange-500 font-semibold">₱ 498.00</p>
        <div class="flex text-gray-800 text-xs mt-1">
          <button
            class="w-5 text-center border border-gray-300 rounded-l-lg pr-1 font-bold"
          >
            -
          </button>
          <p class="w-8 text-end border-y border-gray-300 pr-1 text-gray-800">
            1
          </p>
          <button
            class="w-5 text-center border border-gray-300 rounded-r-lg pr-1 font-bold"
          >
            +
          </button>
        </div>
      </div>
    </div>
    <p>₱ 498.00</p>
  </div>
</template>
