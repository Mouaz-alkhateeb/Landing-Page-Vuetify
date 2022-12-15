<template>
  <section id="project">
    <v-container class="py-15">
      <v-row class="justify-center">
        <v-col class="text-center" lg="12">
          <v-subheader class="text-h4 justify-center teal--text"
            >Projects</v-subheader
          >
          <p>
            Lorem ipsum, dolor sit amet consectetur adipisicing elit. Dolorum,
            laudantium?
          </p>
        </v-col>
        <v-col lg="4" v-for="project in 3" :key="project">
          <v-card class="mx-auto my-12" max-width="374">
            <v-img
              height="250"
              src="https://images.pexels.com/photos/4974912/pexels-photo-4974912.jpeg?auto=compress&cs=tinysrgb&w=600"
            ></v-img>
            <v-card-title>Web Developer</v-card-title>
            <v-card-text>
              <div>
                Small plates, salads & sandwiches - an intimate setting with 12
                indoor seats plus patio seating.
              </div>
            </v-card-text>
            <v-divider class="mx-4"></v-divider>
            <v-card-actions>
              <v-btn small outlined rounded color="teal">
                <v-icon class="mr-2">mdi-eye</v-icon>
                <span>View Details</span>
              </v-btn>
              <v-spacer></v-spacer>
              <v-rating
                :value="3"
                color="amber"
                dense
                half-increments
                readonly
                size="14"
              ></v-rating>
            </v-card-actions>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>

