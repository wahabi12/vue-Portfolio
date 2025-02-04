<template>
    <div class="projects">
      <h1>Mes projets</h1>
      <div class="project-list">
        <div v-for="project in projects" :key="project.id" class="project-card">
          <img :src="project.image" :alt="project.title" />
          <h2>{{ project.title }}</h2>
          <p>{{ project.description }}</p>
          <a :href="project.link" target="_blank" class="btn">Voir le projet</a>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        projects: [
          {
            id: 1,
            title: 'Projet 1',
            description: 'Un projet incroyable réalisé avec Vue.js.',
            image: 'https://via.placeholder.com/300',
            link: '#',
          },
          {
            id: 2,
            title: 'Projet 2',
            description: 'Un autre projet fantastique.',
            image: 'https://via.placeholder.com/300',
            link: '#',
          },
        ],
      };
    },
  };
  </script>
  
  <style scoped>
  .projects {
    padding: 20px;
  }
  .project-list {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
  }
  .project-card {
    background-color: #f9f9f9;
    padding: 20px;
    border-radius: 10px;
    width: 300px;
    text-align: center;
  }
  .project-card img {
    width: 100%;
    border-radius: 10px;
  }
  .btn {
    display: inline-block;
    margin-top: 10px;
    padding: 10px 20px;
    background-color: #42b983;
    color: white;
    text-decoration: none;
    border-radius: 5px;
  }
  </style>