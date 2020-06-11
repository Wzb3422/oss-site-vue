<template>
  <v-app>
    <v-app-bar
      app
      color="orange"
      dark
    >
      <v-app-bar-nav-icon></v-app-bar-nav-icon>
      <v-toolbar-title>Zeb OSS</v-toolbar-title>
    </v-app-bar>

    <v-content>
      <v-card class="d-flex flex-row justify-center mt-12" flat tile>
        <v-card class="d-lg-6 d-sm-12 px-5" raised shaped>
          <v-card-title>Scan QR to Login</v-card-title>
          <v-img class="mb-4" src="https://i.loli.net/2020/06/11/mejz6dPtTquJWli.png" max-width="200"></v-img>
        </v-card>
      </v-card>
    </v-content>
  </v-app>
</template>

<script lang="ts">
import Vue from 'vue';

export default Vue.extend({
  name: 'App',

  components: {
  },

  data: () => ({
    //
  }),
});
</script>
