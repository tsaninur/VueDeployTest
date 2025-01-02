<template>
    <section id="contact" class="contact">
      <h2>Contact Me</h2>
      <form @submit.prevent="submitForm">
        <input type="text" v-model="name" placeholder="Your Name" required />
        <input type="email" v-model="email" placeholder="Your Email" required />
        <textarea v-model="message" placeholder="Your Message" required></textarea>
        <button type="submit">Send</button>
      </form>
    </section>
  </template>
  
  <script>
  export default {
    name: "Contact",
    data() {
      return {
        name: "",
        email: "",
        message: "",
      };
    },
    methods: {
      submitForm() {
        alert(`Message sent by ${this.name}`);
        this.name = "";
        this.email = "";
        this.message = "";
      },
    },
  };
  </script>
  
  <style scoped>
  .contact {
    padding: 50px 20px;
    background-color: #f9f9f9;
    text-align: center;
  }
  form {
    display: flex;
    flex-direction: column;
    max-width: 400px;
    margin: 0 auto;
  }
  form input,
  form textarea {
    margin: 10px 0;
    padding: 10px;
    border: 1px solid #ddd;
    border-radius: 5px;
  }
  form button {
    padding: 10px;
    background-color: #00aced;
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
  }
  form button:hover {
    background-color: #007bb5;
  }
  </style>
  