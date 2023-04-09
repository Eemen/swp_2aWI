<script setup>
  import CardSchnitzel from "./components/CardSchnitzel.vue";
import FooterBottom from "./components/FooterBottom.vue";
  import SideBar from "./components/SideBar.vue"
  import TagesMenue from "./components/TageMenue.vue";

</script>

<template>
  <v-app class="app">
    <SideBar />
    <v-main>
    <CardSchnitzel />
    <TagesMenue />
    <FooterBottom />
    </v-main>
  </v-app>
</template>

<style>
.app{
  background-color: #fff0db;
}
</style>

