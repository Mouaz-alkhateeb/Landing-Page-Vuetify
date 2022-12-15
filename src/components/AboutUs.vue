<template>
  <section id="about">
    <v-container class="py-15">
      <v-row>
        <v-col lg="6">
          <img width="100%" src="../assets/skills.png" />
        </v-col>
        <v-col lg="6">
          <v-subheader class="text-h4 teal--text">About Us</v-subheader>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Debitis
            excepturi dignissimos minus perspiciatis quasi totam nihil
            aspernatur, consequuntur ullam facere dolores eaque deserunt
            obcaecati odio, dolore voluptatibus, veritatis velit aut.
          </p>
          <v-list>
            <v-list-item>
              <v-icon color="primary" class="mr-2">mdi-check-all</v-icon>
              <v-list-item-subtitle
                >Ullamco laboris nisi ut aliquip ex ea commodo
                consequat</v-list-item-subtitle
              >
            </v-list-item>
            <v-list-item>
              <v-icon color="primary" class="mr-2">mdi-check-all</v-icon>
              <v-list-item-subtitle
                >Duis aute irure dolor in reprehenderit in voluptate
                velit</v-list-item-subtitle
              >
            </v-list-item>
            <v-list-item>
              <v-icon color="primary" class="mr-2">mdi-check-all</v-icon>
              <v-list-item-subtitle
                >Ullamco laboris nisi ut aliquip ex ea commodo
                consequat</v-list-item-subtitle
              >
            </v-list-item>
            <v-list-item>
              <v-icon color="primary" class="mr-2">mdi-check-all</v-icon>
              <v-list-item-subtitle
                >Ullamco laboris nisi ut aliquip ex ea commodo
                consequat</v-list-item-subtitle
              >
            </v-list-item>
          </v-list>
          <v-progress-linear
            color="primary"
            buffer-value="0"
            stream
          ></v-progress-linear>
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>

<script>
export default {};
</script>

<style>
</style>