<template>
  <div class="parent">
    <ol>
      <EmployeItem v-for="(employe) in listEmployes" :key="employe.id" :obj="employe" class="employe" />
    </ol>
  </div>
</template>

<script setup>
import { ref } from 'vue';
import EmployeItem from './EmployeItem.vue';

const listEmployes = ref([
  { id: 1, nom: "Aicha", age: 24 }, 
  { id: 2, nom: "Fatima", age: 29 }, 
  { id: 3, nom: "Thillo", age: 20 },
  { id: 4, nom: "Mariam", age: 27 }
])

// function removeEmploye(cpt) {
//   listEmployes.value.splice(cpt, 1)
// }
</script>

<style scoped> 
ol {
  display: flex;
  flex-direction: column;
  gap: 10px;
}

button {
  outline: none;
  color: rgb(6, 37, 51);
  background-color:white ;
  text-align: center;
  font-size: 1em ;
  height: 35px;
}
</style>