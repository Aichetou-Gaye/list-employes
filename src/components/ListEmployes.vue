<template>
    <div>
      <h2>Liste des employés :</h2>
    <ol>
      <li>Employe 1</li>
      <li>Employe 2</li>
      <li>Employe 3</li>
      <li>Employe 4</li>
      </ol>
    </div>
  </template>
  
  <script setup>
  
  </script>
  
  <style scoped>
  div{
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
  