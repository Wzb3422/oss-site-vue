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
      <v-card flat tile>
        <router-view></router-view>
      </v-card>
    </v-content>
  </v-app>
</template>

<script>

export default {
  name: 'Home',
}
</script>
