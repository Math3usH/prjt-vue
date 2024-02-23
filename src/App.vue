<script setup>
import { ref } from 'vue'

const contador = ref(0)

function decrementar() {
  contador.value--
}
function zerar(){
  contador.value = 0
}
</script>

<template>
  <button @click="contador++">+</button>
  <button @click="decrementar">-</button>
  <button @click="zerar">C</button>
  <p>o valor do contador é: {{ contador }}</p>
</template>

<style scoped>
button {
  font-size: 2rem;
  padding: 1rem;
  margin: 1rem;
  cursor: pointer;
  border-radius: 10px;
  
}

button:hover{
  background-color: rgb(99, 99, 99);
}
</style>
