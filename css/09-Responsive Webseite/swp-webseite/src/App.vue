<script setup>
  import CardRezepte from "./components/CardRezepte.vue";
import FooterBottom from "./components/FooterBottom.vue";
  import SideBar from "./components/SideBar.vue"
  import TagesMenue from "./components/TageMenue.vue";

</script>

<template>
  <v-app class="app">
    <SideBar />
    <v-main>
    <CardRezepte />
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

