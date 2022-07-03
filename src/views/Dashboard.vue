<template>
  <div>
    <Navtop />
    <div class="mx-5 my-5">
      <v-row>
        <v-col col="3">
          <v-card elevation="2">
            
          </v-card>
        </v-col>
        <v-col cols="3"> <v-card elevation="2">
            
        </v-card></v-col>
        <v-col cols="3"> <v-card elevation="2"> sss </v-card></v-col>
        <v-col cols="3"> <v-card elevation="2"> sss </v-card></v-col>
      </v-row>
    </div>
  </div>
</template>

<script>
import Navtop from "../components/Navtop.vue";
export default {
  name: "Dashboard",
  components: {
    Navtop,
  },
};
</script>

<style>
</style>