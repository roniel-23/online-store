<script setup>
import CartItem from "./Cart-item.vue";
const emits = defineEmits(["close"]);
</script>

<template>
  <div class="w-full h-full md:h-[70vh] md:w-96 overflow-y-auto bg-white p-2 rounded-lg">
    <div class="flex justify-between items-center border-b pb-2">
      <p class="pl-2">Cart</p>
      <button @click="$emit('close')">
        <img
          src="/images/close.png"
          alt="close"
          class="w-5 p-1 border rounded-lg"
        />
      </button>
    </div>
    <CartItem />
    <CartItem />
    <CartItem />
    <CartItem />
    <div class="sticky bottom-0 w-full flex justify-between p-2 mt-5 bg-white">
        <p class="font-semibold">Total</p>
        <p class="font-semibold">₱ 1098.00</p>
    </div>
  </div>
</template>
