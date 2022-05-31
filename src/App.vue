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
  *{
    font-family: Helvetica, sans-serif;
    padding: 0;
    margin: 0;
    box-sizing: border-box;   
  }

  .main-container {
    margin: 50px;
    min-height: 250px;
  }

  h1 {
    text-align: center;
    font-size: 42px;
    margin-bottom: 30px;
    color: #222;
  }
</style>
