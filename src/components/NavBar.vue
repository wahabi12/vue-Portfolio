<template>
    <nav>
      <router-link to="/">Accueil</router-link>
      <router-link to="/about">À propos</router-link>
      <router-link to="/projects">Projets</router-link>
      <router-link to="/contact">Contact</router-link>
    </nav>
  </template>
  
  <script>
  export default {
    name: 'NavBar',
  };
  </script>
  
  <style scoped>
  nav {
    background-color: #42b983;
    padding: 10px;
    text-align: center;
  }
  nav a {
    color: white;
    margin: 0 10px;
    text-decoration: none;
  }
  nav a.router-link-exact-active {
    font-weight: bold;
  }
  </style>