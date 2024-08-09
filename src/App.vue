<template>
  <h1>Liste des employés</h1>
  <div class="wrapper">
    <ListEmployes/>
  </div>
</template>

<script setup>
import ListEmployes from './components/ListEmployes.vue';
</script>

<style scoped>
h1{
  font-family: Poppins;
  text-align: center;
}
</style>
