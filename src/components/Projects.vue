<template>
    <section id="projects" class="projects">
      <h2>My Projects</h2>
      <div class="project-list">
        <div class="project" v-for="project in projects" :key="project.id">
          <h3>{{ project.name }}</h3>
          <p>{{ project.description }}</p>
          <a :href="project.link" target="_blank">View Project</a>
        </div>
      </div>
    </section>
  </template>
  
  <script>
  export default {
    name: "Projects",
    data() {
      return {
        projects: [
          {
            id: 1,
            name: "Project One",
            description: "A brief description of project one.",
            link: "https://example.com/project-one",
          },
          {
            id: 2,
            name: "Project Two",
            description: "A brief description of project two.",
            link: "https://example.com/project-two",
          },
        ],
      };
    },
  };
  </script>
  
  <style scoped>
  .projects {
    padding: 50px 20px;
  }
  .project-list {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
  }
  .project {
    border: 1px solid #ddd;
    padding: 20px;
    border-radius: 8px;
    flex: 1 1 calc(50% - 20px);
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  }
  .project h3 {
    font-size: 1.5rem;
    margin-bottom: 10px;
  }
  .project a {
    text-decoration: none;
    color: #00aced;
    font-weight: bold;
  }
  </style>
  