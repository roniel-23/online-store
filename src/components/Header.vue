<script setup>
const emits = defineEmits(["cart"]);
</script>

<template>
  <div class="max-w-7xl mx-auto flex items-center px-2 md:px-0 py-4 justify-between">
    <div class="flex items-center">
      <img src="/antego.png" alt="Antego Logo" class="w-16 mr-2" />
      <p class="hidden sm:inline text-xl font-light">Antego Solutions</p>
    </div>
    <div>
        <!-- <button @click="$emit('cart')" class="font-light">Cart</button> -->
        <button @click="$emit('cart')" class="font-light flex items-center space-x-2">
            <img src="/images/shopping-cart.png" alt="cart" class="w-4 aspect-square">
            <p class="font-light">My Cart</p>
        </button>
    </div>
  </div>
</template>
