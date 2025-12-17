<template>
  <main class="container">
    <h1>💙 Málaga CF</h1>

    <ul>
      <li>Estadio: La Rosaleda</li>
      <li>Ciudad: Málaga</li>
      <li>Colores: Azul y Blanco</li>
      <li>Entrenador: Sergio Pellicer</li>
    </ul>

    <button @click="mostrar = !mostrar">
      {{ mostrar ? "Ocultar" : "Mostrar" }} lema
    </button>

    <p v-if="mostrar" class="lema">Siempre Málaga 💙</p>
  </main>
</template>

<script setup>
import { ref } from "vue";
const mostrar = ref(false);
</script>

<style scoped>
.container {
  font-family: Arial, sans-serif;
  max-width: 600px;
  margin: 40px auto;
  text-align: center;
}

h1 {
  color: #0056a3;
}

button {
  margin-top: 20px;
  padding: 8px 12px;
}

.lema {
  margin-top: 10px;
  font-weight: bold;
}

ul {
  list-style-type: none;
  padding-left: 0;
  margin-left: 0;
}

li {
  list-style-type: none;
}
</style>
