<template>
  <v-footer padless>
    <v-card class="flex text-center grey lighten-4" flat>
      <v-card-title class="justify-center">
        <v-btn
          v-for="(icon, i) in icons"
          :key="i"
          class="mx-4"
          color="white"
          text
          fab
        >
          <v-icon size="24px" large :color="icon.color">
            {{ icon.name }}
          </v-icon>
        </v-btn>
      </v-card-title>
      <v-divider class="mx-4"></v-divider>
      <v-card-text class="py-2 text-center">
        <strong class="font-weight-bold">Design By Mouaz Alkhateeb</strong>
        --{{ new Date().getFullYear() }}
      </v-card-text>
    </v-card>
  </v-footer>
</template>

<script>
export default {
  data() {
    return {
      icons: [
        { name: "mdi-facebook", color: "blue" },
        { name: "mdi-twitter", color: "blue" },
        { name: "mdi-instagram", color: "red" },
        { name: "mdi-google", color: "red" },
        { name: "mdi-linkedin", color: "blue" },
      ],
    };
  },
};
</script>