<template>
  <div class="about">
    <h1>This is an about page</h1>
  </div>
  <br>
  <div>
    <p>Contador: {{ counter.count }}</p>
    <p>Dobro: {{ counter.doubleCount }}</p>
    <button @click="counter.increment">Aumentar</button>
    <button @click="counter.reset">Zerar</button>

    

  </div>
</template>

<script setup>
 import { useCounterStore } from '@/stores/useCounterStore'
 const counter = useCounterStore()
</script>