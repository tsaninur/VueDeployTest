<template>
    <header class="header">
      <nav>
        <ul>
          <li><a href="#about">About</a></li>
          <li><a href="#projects">Projects</a></li>
          <li><a href="#skills">Skills</a></li>
          <li><a href="#contact">Contact</a></li>
        </ul>
      </nav>
    </header>
  </template>
  
  <script>
  export default {
    name: "Header",
  };
  </script>
  
  <style scoped>
  .header {
    background-color: #333;
    color: #fff;
    padding: 10px 20px;
    position: sticky;
    top: 0;
    z-index: 1000;
  }
  nav ul {
    list-style: none;
    display: flex;
    justify-content: space-around;
    margin: 0;
    padding: 0;
  }
  nav a {
    text-decoration: none;
    color: #fff;
    font-weight: bold;
  }
  nav a:hover {
    color: #00aced;
  }
  </style>
  