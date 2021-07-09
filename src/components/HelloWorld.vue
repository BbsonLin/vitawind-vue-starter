<template>
  <h1 class="text-4xl font-semibold">{{ msg }}</h1>

  <p class="text-lg">
    <a href="https://vitejs.dev/guide/features.html" target="_blank">
      Vite Documentation
    </a>
    |
    <a href="https://v3.vuejs.org/" target="_blank">Vue 3 Documentation</a>
    |
    <a href="https://vitawind-blog.vercel.app/" target="_blank">Vitawind Documentation</a>
  </p>
  <div class="my-10">
    <p class="text-xl font-semibold">Count Button with TailwindCSS</p>
    <button type="button" class="py-2 px-4 border-2 border-blue-300 shadow-sm active:shadow-lg focus:bg-blue-400" @click="state.count++">Click Me : {{ state.count }}</button>
  </div>
  <p>
    Edit
    <code>components/HelloWorld.vue</code> to test hot module replacement.
  </p>
</template>

<script setup>
import { defineProps, reactive } from 'vue'

defineProps({
  msg: String
})

const state = reactive({ count: 0 })
</script>

<style scoped>
a {
  color: #11b6c6;
}
</style>
