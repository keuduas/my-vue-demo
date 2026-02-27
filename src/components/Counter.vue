<template>
  <div class="max-w-sm mx-auto my-8 p-8 border-2 border-emerald-500 rounded-lg text-center">
    <h2 class="text-2xl font-bold mb-4">计数器</h2>
    <div class="text-5xl font-bold text-emerald-500 my-6">{{ count }}</div>
    <div class="flex gap-4 justify-center">
      <button @click="decrement" class="px-6 py-2 text-xl bg-emerald-500 text-white rounded hover:bg-slate-700 active:scale-95 transition">-</button>
      <button @click="reset" class="px-6 py-2 text-xl bg-emerald-500 text-white rounded hover:bg-slate-700 active:scale-95 transition">重置</button>
      <button @click="increment" class="px-6 py-2 text-xl bg-emerald-500 text-white rounded hover:bg-slate-700 active:scale-95 transition">+</button>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const count = ref(0)

const increment = () => {
  count.value++
}

const decrement = () => {
  if (count.value > 0) {
    count.value--
  }
}

const reset = () => {
  count.value = 0
}
</script>
