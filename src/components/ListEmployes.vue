<template>
  <div>
    <ol>
      <li v-for="(employe, cpt) in listEmployes" :key="employe.id">
        {{ employe.nom }} - <button type="button" @click="removeEmploye(cpt)">Remove</button>
      </li>
    </ol>
  </div>
</template>

<script setup>
import { ref } from 'vue';

const listEmployes = ref([
  { id: 1, nom: "Aicha", age: 24 }, 
  { id: 2, nom: "Fatima", age: 29 }, 
  { id: 3, nom: "Thillo", age: 20 },
  { id: 4, nom: "Mariam", age: 27 }
])

function removeEmploye(cpt) {
  listEmployes.value.splice(cpt, 1)
}
</script>

<style scoped>
div {
  border: 2px solid rgba(131, 203, 212, 0.933);
  border-radius: 5px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  width: 500px;
  margin: auto;
  background-color: rgb(230, 237, 240);
  padding: 20px;
}

ol {
  display: flex;
  flex-direction: column;
}

li {
  font-family: sans-serif;
  font-size: 1.2em;
  color: black;
  height: 50px;
}

li:hover {
  background-color: rgb(6, 37, 51);
  color: white;
}
</style>