<script setup>
import { ref } from 'vue'

defineProps({
  msg: String
})

const count = ref(0)
</script>

<template>
  <h1 class="
    text-red-700 font-extrabold text-6xl
    bg-clip-text text-transparent bg-gradient-to-r from-cyan-500 to-blue-300
    mb-10 
    "
  >
    {{ msg }}
  </h1>

  <div class="flex flex-row flex-wrap gap-1">
    <div 
      v-for="(item, index) in 1000" :key="index"

      class="
        w-4 h-4
        bg-gradient-to-r from-cyan-500 to-blue-300
        hover:bg-gradient-to-r hover:from-white hover:to-red-300
      "
    >
    </div>
    
  </div>
  



  
</template>

<style scoped>
a {
  color: #42b983;
}
</style>
