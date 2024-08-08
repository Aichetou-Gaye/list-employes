<template>
    <div>
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
    display: flex;
    justify-content: center;
    width: 600px;
    margin: 0 20%;
    background-color: rgb(236, 226, 177);
  }
  ol {
    display: flex;
    flex-direction: column;
    gap: 50px;
  }
  li {
    font-family: sans-serif;
    font-size: 1.5em;
    color: black;
  }
  li:hover {
    background-color: rgb(88, 42, 48);
    color: white;
  }
  </style>
  