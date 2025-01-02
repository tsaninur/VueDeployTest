<template>
    <section id="skills" class="skills">
      <h2>My Skills</h2>
      <ul>
        <li v-for="skill in skills" :key="skill">{{ skill }}</li>
      </ul>
    </section>
  </template>
  
  <script>
  export default {
    name: "Skills",
    data() {
      return {
        skills: ["HTML", "CSS", "JavaScript", "Vue.js", "Git", "Node.js"],
      };
    },
  };
  </script>
  
  <style scoped>
  .skills {
    background-color: #f0f8ff;
    padding: 50px 20px;
    text-align: center;
  }
  .skills ul {
    list-style: none;
    padding: 0;
  }
  .skills li {
    display: inline-block;
    margin: 10px;
    padding: 10px 20px;
    background-color: #00aced;
    color: white;
    border-radius: 20px;
    font-weight: bold;
  }
  </style>
  