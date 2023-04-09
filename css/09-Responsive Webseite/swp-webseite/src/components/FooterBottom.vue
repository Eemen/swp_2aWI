<template>
    <v-footer class="fotter-wrapper">
      <v-row justify="center" no-gutters>
        <v-btn
          v-for="link in links"
          :key="link"
          color="white"
          variant="text"
          class="mx-2"
          rounded="xl"
        >
          {{ link }}
        </v-btn>
        <v-col class="text-center mt-4" cols="12">
        </v-col>
      </v-row>
    </v-footer>
  </template>


<script>
  export default {
    data: () => ({
      links: [
        'Impressum',
        'Über uns',
        'Team',
        'Datanschutz',
      ],
    }),
  }
</script>

<style>
.fotter-wrapper{
    background-color: #e6d2b8;
    margin-top: 40px;
}


</style>