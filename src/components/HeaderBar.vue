<template>
  <v-app-bar
    app
    color="white"
    light
    elevate-on-scroll
    elevation="6"
    style="padding: 0px 90px"
  >
    <v-toolbar-title class="Titleproject"> My Project </v-toolbar-title>
    <v-spacer></v-spacer>
    <v-btn text @click="$vuetify.goTo('#hero')" rounded color="teal">
      <span class="mr-2">Home</span>
    </v-btn>
    <v-btn text @click="$vuetify.goTo('#about')" rounded color="teal">
      <span class="mr-2">About Us</span>
    </v-btn>
    <v-btn text @click="$vuetify.goTo('#portfolio')" rounded color="teal">
      <span class="mr-2">Protfolio</span>
    </v-btn>
    <v-btn text @click="$vuetify.goTo('#project')" rounded color="teal">
      <span class="mr-2">Projects</span>
    </v-btn>
    <v-btn text @click="$vuetify.goTo('#gallery')" rounded color="teal">
      <span class="mr-2">Gallery</span>
    </v-btn>
    <v-btn text @click="$vuetify.goTo('#contact')" rounded color="teal">
      <span class="mr-2">Contct Us</span>
    </v-btn>

    <v-btn rounded color="teal" class="white--text ml-2"> Get Started </v-btn>
  </v-app-bar>
</template>
<script>
export default {
  name: "App",
};
</script>
<style  scoped>
.Titleproject {
  font-size: 32px;
  font-weight: 700;
  font-family: cursive;
  color: #009688;
}
</style>