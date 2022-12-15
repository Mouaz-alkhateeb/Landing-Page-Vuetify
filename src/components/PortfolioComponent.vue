<template>
  <section id="portfolio">
    <v-container class="py-15">
      <v-row class="justify-center">
        <v-col class="text-center" lg="12">
          <v-subheader class="text-h4 justify-center teal--text">Portfolio</v-subheader>
          <p>
            Lorem ipsum, dolor sit amet consectetur adipisicing elit. Dolorum,
            laudantium?
          </p>
        </v-col>
        <v-col lg="12">
          <div class="text-center">
            <v-chip
              class="mx-5"
              :color="activeProtofile == 'webapp' ? 'primary' : ''"
              @click="activeProtofile = 'webapp'"
              outlined
              >Web Application</v-chip
            >
            <v-chip
              class="mx-5"
              :color="activeProtofile == 'mobileapp' ? 'success' : ''"
              @click="activeProtofile = 'mobileapp'"
              outlined
              >Mobile Application</v-chip
            >
            <v-chip
              class="mx-5"
              :color="activeProtofile == 'desktopapp' ? 'red' : ''"
              @click="activeProtofile = 'desktopapp'"
              outlined
              >Desktop Application</v-chip
            >
          </div>
        </v-col>
        <slot v-if="activeProtofile == 'webapp'">
          <v-col lg="3" v-for="(card, index) in webapp" :key="index">
            <v-card>
              <v-img
                :src="card.image"
                class="white--text align-end"
                gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
                height="200px"
              >
                <v-card-title>{{ card.title }}</v-card-title>
              </v-img>
            </v-card>
          </v-col>
        </slot>
        <slot v-if="activeProtofile == 'mobileapp'">
          <v-col lg="3" v-for="(card, index) in mobileapp" :key="index">
            <v-card>
              <v-img
                :src="card.image"
                class="white--text align-end"
                gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
                height="200px"
              >
                <v-card-title>{{ card.title }}</v-card-title>
              </v-img>
            </v-card>
          </v-col>
        </slot>
        <slot v-if="activeProtofile == 'desktopapp'">
          <v-col lg="3" v-for="(card, index) in desktopapp" :key="index">
            <v-card>
              <v-img
                :src="card.image"
                class="white--text align-end"
                gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
                height="200px"
              >
                <v-card-title>{{ card.title }}</v-card-title>
              </v-img>
            </v-card>
          </v-col>
        </slot>
      </v-row>
    </v-container>
  </section>
</template>

<script>
export default {
  data() {
    return {
      activeProtofile: "webapp",
      webapp: [
        {
          title: "App 1",
          image:
            "https://images.pexels.com/photos/5899079/pexels-photo-5899079.jpeg?auto=compress&cs=tinysrgb&w=600",
          flex: 12,
        },
        {
          title: "App 2",
          image:
            "https://images.pexels.com/photos/6044806/pexels-photo-6044806.jpeg?auto=compress&cs=tinysrgb&w=600",
          flex: 12,
        },
        {
          title: "App 10",
          image:
            "https://images.pexels.com/photos/990423/pexels-photo-990423.jpeg?auto=compress&cs=tinysrgb&w=600",
          flex: 12,
        },
        {
          title: "App 11",
          image:
            "https://images.pexels.com/photos/6986561/pexels-photo-6986561.jpeg?auto=compress&cs=tinysrgb&w=600",
          flex: 12,
        },
        {
          title: "App 3",
          image:
            "https://images.pexels.com/photos/6368894/pexels-photo-6368894.jpeg?auto=compress&cs=tinysrgb&w=600",
          flex: 12,
        },
        {
          title: "App 4",
          image:
            "https://images.pexels.com/photos/3846554/pexels-photo-3846554.jpeg?auto=compress&cs=tinysrgb&w=600",
          flex: 12,
        },
      ],
      mobileapp: [
        {
          title: "App 5",
          image:
            "https://images.pexels.com/photos/5273662/pexels-photo-5273662.jpeg?auto=compress&cs=tinysrgb&w=600",
          flex: 12,
        },
        {
          title: "App 10",
          image:
            "https://images.pexels.com/photos/990423/pexels-photo-990423.jpeg?auto=compress&cs=tinysrgb&w=600",
          flex: 12,
        },
        {
          title: "App 11",
          image:
            "https://images.pexels.com/photos/6986561/pexels-photo-6986561.jpeg?auto=compress&cs=tinysrgb&w=600",
          flex: 12,
        },
        {
          title: "App 6",
          image:
            "https://images.pexels.com/photos/5668862/pexels-photo-5668862.jpeg?auto=compress&cs=tinysrgb&w=600",
          flex: 12,
        },
        {
          title: "App 7",
          image:
            "https://images.pexels.com/photos/7731358/pexels-photo-7731358.jpeg?auto=compress&cs=tinysrgb&w=600",
          flex: 13,
        },
        {
          title: "App 8",
          image:
            "https://images.pexels.com/photos/5668793/pexels-photo-5668793.jpeg?auto=compress&cs=tinysrgb&w=600",
          flex: 14,
        },
      ],
      desktopapp: [
        {
          title: "App 9",
          image:
            "https://images.pexels.com/photos/5499551/pexels-photo-5499551.jpeg?auto=compress&cs=tinysrgb&w=600",
          flex: 12,
        },
        {
          title: "App 10",
          image:
            "https://images.pexels.com/photos/990423/pexels-photo-990423.jpeg?auto=compress&cs=tinysrgb&w=600",
          flex: 12,
        },
        {
          title: "App 11",
          image:
            "https://images.pexels.com/photos/6986561/pexels-photo-6986561.jpeg?auto=compress&cs=tinysrgb&w=600",
          flex: 12,
        },
        {
          title: "App 12",
          image:
            "https://images.pexels.com/photos/5696224/pexels-photo-5696224.jpeg?auto=compress&cs=tinysrgb&w=600",
          flex: 12,
        },
        {
          title: "App 6",
          image:
            "https://images.pexels.com/photos/5668862/pexels-photo-5668862.jpeg?auto=compress&cs=tinysrgb&w=600",
          flex: 12,
        },
        {
          title: "App 7",
          image:
            "https://images.pexels.com/photos/7731358/pexels-photo-7731358.jpeg?auto=compress&cs=tinysrgb&w=600",
          flex: 13,
        },
      ],
    };
  },
};
</script>

<style>
</style>