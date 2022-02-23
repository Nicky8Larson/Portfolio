<template>
  <v-app-bar app color="#111111" dark flat class="px-8">
    <v-btn icon @click="scroll('home')">
      <v-icon color="#2465aa">fas fa-dragon</v-icon>
    </v-btn>

    <v-spacer></v-spacer>
    <v-btn text @click="scroll('home')">Accueil</v-btn>
    <v-btn text @click="scroll('project')">Projets</v-btn>
    <v-btn text @click="scroll('contact')">Contact</v-btn>
  </v-app-bar>
</template>

<script>
export default {
  methods: {
    scroll(refName) {
      const element = document.getElementById(refName);
      element.scrollIntoView({ behavior: "smooth" });
    },
  },
};
</script>

<style></style>
