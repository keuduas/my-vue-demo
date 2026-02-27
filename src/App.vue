<script setup>
</script>

<template>
  <div class="min-h-screen bg-gray-50">
    <nav class="p-4 text-center bg-gray-100 shadow">
      <router-link to="/" class="mx-4 font-bold text-emerald-500 hover:text-slate-700 transition">首页</router-link>
      <router-link to="/about" class="mx-4 font-bold text-emerald-500 hover:text-slate-700 transition">关于</router-link>
    </nav>
    <router-view />
  </div>
</template>
