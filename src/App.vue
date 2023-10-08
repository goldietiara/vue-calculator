<script setup>
import { ref } from "vue";

const count = ref(0);
</script>

<template>
  <main class="flex w-full h-screen items-center justify-center bg-black">
    <div
      class="grid grid-cols-3 w-[400px] h-[400px] items-center justify-center bg-pink-50 text-pink-500 text-3xl text-center"
    >
      <h1 class="col-span-3">The current count is ..</h1>
      <p class="col-span-3 text-5xl">{{ count }}</p>
      <button
        class="h-full text-pink-50 bg-pink-400 hover:bg-pink-500 transition-all ease-in-out duration-100 active:text-xl"
        @click="count--"
      >
        -
      </button>
      <button
        class="h-full text-pink-50 bg-pink-400 hover:bg-pink-500 transition-all ease-in-out duration-100 active:text-xl"
        @click="count++"
      >
        +
      </button>
      <button
        class="h-full text-pink-50 bg-pink-400 hover:bg-pink-500 transition-all ease-in-out duration-100 active:text-xl"
        @click="count = 0"
      >
        reset
      </button>
    </div>
  </main>
</template>
