<script>
import { RouterLink, RouterView } from "vue-router";
import Navbar from "@/components/Navbar.vue";
import Footer from "@/components/Footer.vue";

export default {
  components: {
    Navbar,
    Footer
  },
  data() {
    return { 
      logo_src: "/img/logo.png",
      app_name: "Make Your Burger"
     }
  }
}

</script>

<template>
  <header>
    <!-- <img
      alt="Vue logo"
      class="logo"
      src="@/assets/logo.svg"
      width="125"
      height="125"
    /> -->

    <div class="wrapper">
      <Navbar :logo="logo_src" :alt="app_name"></Navbar>
      <Footer></Footer>
    </div>
  </header>
</template>

<style>
</style>
