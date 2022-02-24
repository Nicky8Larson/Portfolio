<template>
  <v-footer dark padless>
    <v-card
      flat
      tile
      class="black white--text py-5 px-5 text-center"
      width="100%"
    >
      <v-row>
        <v-col cols="12" sm="4">
          <v-card-text class="white--text pt-2">
            <v-btn icon>
              <v-icon color="#2465aa">fas fa-dragon</v-icon>
            </v-btn>
          </v-card-text>
        </v-col>

        <v-col cols="12" sm="4">
          <v-card-text class="pt-2">
            <v-btn
              v-for="icon in icons"
              :key="icon.id"
              class="mx-1 white--text"
              icon
              :href="icon.url"
              target="_blank"
            >
              <v-icon size="24px">
                {{ icon.name }}
              </v-icon>
            </v-btn>
          </v-card-text>
        </v-col>
        <v-col cols="12" sm="4">
          <v-card-text class="pt-2">
            <v-btn class="mx-1 white--text" icon>
              <v-icon color="#A7121D">mdi-heart</v-icon>
            </v-btn>
            Created by Sammy Merazga
          </v-card-text>
        </v-col>
      </v-row>
    </v-card>
  </v-footer>
</template>

<script>
export default {
  data() {
    return {
      icons: [
        {
          id: 1,
          name: "fab fa-github",
          url: "https://github.com/SammyMERAZGA"
        },
        {
          id: 2,
          name: "fab fa-linkedin",
          url: "https://fr.linkedin.com/in/sammy-merazga",
        },
        {
          id: 3,
          name: "fas fa-envelope",
          url: "mailto:sammy.merazga@gmail.com"
        }
      ]
    };
  },
};
</script>

<style></style>
