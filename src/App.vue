<template>
  <v-app>
    <header-bar />
    <v-main>
      <hero-component />
      <about-us />
      <portfolio-component />
      <project-component />
      <gallery-components />
      <contact-us />
      <v-btn
        v-scroll="onScroll"
        v-show="fab"
        fab
        dark
        fixed
        bottom
        right
        color="teal"
        @click="toTop"
      >
        <v-icon>mdi-arrow-up-thick</v-icon>
      </v-btn>
      <footer-component />
      <router-view />
    </v-main>
  </v-app>
</template>

<script>
import HeaderBar from "./components/HeaderBar.vue";
import HeroComponent from "./components/HeroComponent.vue";
import AboutUs from "./components/AboutUs.vue";
import PortfolioComponent from "./components/PortfolioComponent.vue";
import ProjectComponent from "./components/ProjectComponent.vue";
import GalleryComponents from "./components/GalleryComponents.vue";
import ContactUs from "./components/ContactUs.vue";
import FooterComponent from "./components/FooterComponent.vue";
export default {
  name: "App",
  data() {
    return {
      fab: false,
    };
  },
  components: {
    HeaderBar,
    HeroComponent,
    AboutUs,
    PortfolioComponent,
    ProjectComponent,
    GalleryComponents,
    ContactUs,
    FooterComponent,
  },
  methods: {
    onScroll(e) {
      if (typeof window === "undefined") return;
      const top = window.pageYOffset || e.target.scrollTop || 0;
      this.fab = top > 20;
    },
    toTop() {
      this.$vuetify.goTo("#hero");
    },
  },
};
</script>


