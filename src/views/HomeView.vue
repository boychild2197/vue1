<template>
  <div>
      <Topbar />
      <HomeBody />
  </div>

</template>

<script>
import Topbar from "../components/Topbar";
import HomeBody from "../components/HomeBody.vue"

export default {
  name: "Home",

  components: {
    Topbar,
    HomeBody
  },
};
</script>
