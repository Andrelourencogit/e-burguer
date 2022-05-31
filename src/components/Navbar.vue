<script setup>
import { RouterLink, RouterView } from "vue-router";
defineProps([
    'logo',
    'alt'
])
</script>

<template>
  <div>
    <div id="nav">
      <RouterLink id="logo-url" to="/"><img id="logo" :src="logo" :alt="alt"></RouterLink>
      <RouterLink to="/">Home</RouterLink>
      <RouterLink to="/pedidos">Pedidos</RouterLink>
    </div>
  </div>
  <RouterView />
</template>

<style scoped>
  #nav {
    background-color: #222;
    border-bottom: 4px solid #111;
    padding: 15px 50px;
    display: flex;
    justify-content: flex-end;
    align-items: center;
  }
  #nav #logo-url {
    margin: auto;
    margin-left: 0;
  }
  #logo {
    width: 40px;
    height: 40px;
  }
  #nav a {
    color: #fcba03;
    text-decoration: none;
    margin: 12px;
    transition: .5s;
  }
  #nav a:hover {
    color: #FFF;
  }
</style>