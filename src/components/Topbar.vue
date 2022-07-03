<template>
  <v-app-bar app color="primary"  flat>
    <v-toolbar color="primary" flat>
      <!-- <v-app-bar-nav-icon></v-app-bar-nav-icon> -->
      <v-spacer></v-spacer>
      <v-toolbar-title class="white--text font-weight-bold display-1"
        >Universal Payment system</v-toolbar-title
      >

      <v-spacer></v-spacer>

      <v-btn class="primary--text"
        ><router-link style="text-decoration: none" to="/login"
          >Login</router-link
        >
      </v-btn>

      <v-btn class="mx-5 primary--text"
        ><router-link style="text-decoration: none" to="/register"
          >Register</router-link
        >
      </v-btn>
    </v-toolbar>
  </v-app-bar>
</template>

<script>
export default {
  name: "Topbar",

  data: () => ({}),
};
</script>
