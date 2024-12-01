<script setup>
import { ref } from 'vue';
import Header from "./components/Header.vue";
import Item from "./components/Item.vue";
import Cart from "./components/Cart.vue";

var showCart = ref(false);
const categories = ["Arduino", "IOT", "Solar", "Peripherals"];
</script>

<template>
  <div class="bg-gray-100">
    <Header @cart="showCart = !showCart"> </Header>
    <div class="max-w-7xl mx-auto">
      <Cart v-if="showCart" @close="showCart = !showCart" class=" z-10 fixed md:right-28"/>
    </div>
    <div class="max-w-7xl mx-auto grid md:grid-cols-6 relative">
      <div class="hidden sm:inline col-span-1 sticky top-5 h-fit">
        <h2 class="font-semibold text-sm mb-1">Category</h2>
        <button
          v-for="category in categories"
          class="grid pl-2 text-gray-600 hover:text-orange-600 transition-colors font-light"
        >
          {{ category }}
        </button>
      </div>
      <div class="col-span-5 grid grid-cols-2 md:grid-cols-5">
        <Item />
        <Item />
        <Item />
        <Item />
        <Item />
        <Item />
        <Item />
        <Item />
        <Item />
        <Item />
        <Item />
        <Item />
        <Item />
      </div>
    </div>
  </div>
</template>
