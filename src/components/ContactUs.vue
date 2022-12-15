<template>
  <section id="contact">
    <v-container class="py-15">
      <v-row class="justify-center">
        <v-col class="text-center" lg="12">
          <v-subheader class="text-h4 justify-center teal--text"
            >Contact Us</v-subheader
          >
          <p>
            Lorem ipsum, dolor sit amet consectetur adipisicing elit. Dolorum,
            laudantium?
          </p>
        </v-col>
        <v-col lg="6">
          <iframe
            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d425061.75903789914!2d36.33988932561612!3d33.66247348404516!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x1518e6dc413cc6a7%3A0x6b9f66ebd1e394f2!2z2K_Zhdi02YLYjCDYs9mI2LHZitin!5e0!3m2!1sar!2s!4v1671043221688!5m2!1sar!2s"
            width="100%"
            height="400"
            style="border: 0"
            allowfullscreen=""
            loading="lazy"
            referrerpolicy="no-referrer-when-downgrade"
          ></iframe>
        </v-col>
        <v-col lg="6">
          <form ref="form">
            <v-text-field label="Name" v-model="name"></v-text-field>
            <v-text-field
              label="E-mail"
              v-model="email"
              class="mb-3"
            ></v-text-field>
            <v-textarea label="Message" v-model="message" rows="5"></v-textarea>
            <v-btn color="success" outlined rounded class="justify-center">
              Send
            </v-btn>
          </form>
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>
<script>
export default {
  data() {
    return {
      name: "",
      email: "",
      message: "",
    };
  },
};
</script>

