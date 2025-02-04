<template>
    <div class="home">
      <h1>Bienvenue sur mon portfolio</h1>
      <p>Je suis un passionné de développement web spécialisé en Vue.js.</p>
      <router-link to="/about" class="btn">En savoir plus</router-link>
    </div>
  </template>
  
  <script>
  export default {
    name: 'HomeView',
  };
  </script>
  
  <style scoped>
  .home {
    text-align: center;
    padding: 50px;
  }
  .btn {
    display: inline-block;
    margin-top: 20px;
    padding: 10px 20px;
    background-color: #42b983;
    color: white;
    text-decoration: none;
    border-radius: 5px;
  }
  </style>