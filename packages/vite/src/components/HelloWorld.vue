<script setup>
import { ref } from 'vue'

defineProps({
  msg: String,
})

const count = ref(0)
</script>

<template>
  <div
    class="min-h-screen bg-gray-50 py-6 flex flex-col justify-center relative overflow-hidden sm:py-12"
  >
    <h1 class="text-3xl font-bold text-center">{{ msg }}</h1>
    <hr />
    <button
      class="border mx-auto rounded-md w-64 p-5 hover:bg-slate-400 hover:text-slate-100"
      type="button"
      @click="count++"
    >
      count is: {{ count }}
    </button>
  </div>
</template>

<style scoped>
hr {
  box-sizing: content-box;
  border: 0;
  line-height: 1.25em;
  margin: 6px;
  height: 0.0625rem;
  background: linear-gradient(
    to right,
    transparent,
    #000 30%,
    #000 70%,
    transparent
  );
}
</style>
