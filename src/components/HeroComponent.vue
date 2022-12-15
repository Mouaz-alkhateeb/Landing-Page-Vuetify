<template>
  <section id="hero">
    <v-container class="py-15">
      <v-row>
        <v-col lg="6">
          <h2 class="intro-text">Welcome To Our Compamy</h2>
          <p class="description">
            Lorem ipsum dolor sit amet consectetur adipisicing elit.
            Reprehenderit sint odio, tenetur totam eum velit adipisci enim saepe
            culpa facilis? Error sunt iure labore quod obcaecati fuga, molestiae
            similique sed?
          </p>

          <v-btn outlined rounded color="primary" class="white--text">
            <v-icon class="mr-2">mdi-youtube-tv</v-icon> Watch Video
          </v-btn>
        </v-col>
        <v-col lg="6">
          <img width="100%" src="../assets/hero-img.png" />
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>

<script>
export default {};
</script>

<style  scoped>
h2.intro-text {
  font-size: 60px;
  font-weight: bold;
  font-family: cursive;
  color: #444;
}
p.description {
  font-size: 19px;
  font-family: cursive;
  margin: 32px 0px;
  color: #444444ba;
}
</style>