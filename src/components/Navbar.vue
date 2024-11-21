<template>
    <v-app-bar app color="#111111" dark flat class="px-8">
      <v-btn icon>
        <v-icon color="#A7121D">fas fa-dragon</v-icon>
      </v-btn>
  
      <v-spacer></v-spacer>
      <v-btn text @click="scroll('home')">Home</v-btn>
      <v-btn text @click="scroll('project')">Projetos</v-btn>
      <v-btn text @click="scroll('about')">Sobre</v-btn>
      <v-btn text @click="scroll('contact')"> Contato</v-btn>
    </v-app-bar>
  </template>
  
  <script>
  export default {
    name: 'NavbarApp',
    methods: {
      scroll(refName) {
        const element = document.getElementById(refName);
        element.scrollIntoView({ behavior: "smooth" });
      },
    },
  };
  </script>
  
  <style>
  </style>