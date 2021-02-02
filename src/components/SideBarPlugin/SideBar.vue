<template>
  <nav>
    <v-toolbar flat app>
      <!-- <v-toolbar-side-icon class="grey--text" @click="drawer= !drawer"></v-toolbar-side-icon> -->
      <v-app-bar-nav-icon
        class="grey--text"
        @click="drawer = !drawer"
      ></v-app-bar-nav-icon>
      
      <v-toolbar-title class="text-uppercase grey--text">
        <p class="font-weight-light">Give me a car</p>
        <p class="font-weight-light">Admin</p>
      </v-toolbar-title>
    </v-toolbar>

    <v-navigation-drawer app v-model="drawer" class="indigo">
      <br />
      <p class="display-1 white--text">Stock</p>
      <!-- <v-btn fab small>
        <v-icon>mdi-menu</v-icon>
        </v-btn> -->
    </v-navigation-drawer>
  </nav>
</template>


<script>
export default {
  data() {
    return {
      drawer: false,
    };
  },
};
</script>