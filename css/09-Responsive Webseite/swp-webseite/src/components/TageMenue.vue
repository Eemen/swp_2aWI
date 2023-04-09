<template>
    <v-card
      class="wrapper"
      max-width="500"
    >
    <p class="favuberschrift" id="tag">Unser Tages Menü</p>
      <v-container fluid>
        <v-row dense>
          <v-col
            v-for="card in cards"
            :key="card.title"
            :cols="card.flex"
          >
            <v-card>
              <v-img
                :src="card.src"
                class="align-end"
                gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
                height="200px"
                cover
              >
                <v-card-title class="text-white" v-text="card.title"></v-card-title>
              </v-img>
  
              <v-card-actions>
                <v-spacer></v-spacer>
  
                <v-btn size="small" color="surface-variant" variant="text" icon="mdi-heart"></v-btn>
  
                <v-btn size="small" color="surface-variant" variant="text" icon="mdi-bookmark"></v-btn>
  
                <v-btn size="small" color="surface-variant" variant="text" icon="mdi-share-variant"></v-btn>
              </v-card-actions>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </v-card>
  </template>


<script>
  export default {
    data: () => ({
      cards: [
        { title: 'Lachs aus dem Ofen', src: 'https://image.livingathome.de/12878842/t/ou/v2/w960/r1/-/lah200702-lachs-aus-dem-ofen-mit-dill-jpg--51084-.jpg', flex: 12 },
        { title: 'Tomaten-Aprikosen-Suppe', src: 'https://image.livingathome.de/12859600/t/zT/v2/w960/r1/-/lah201507080-tomaten-aprikosen-suppe-jpg--42338-.jpg', flex: 6 },
        { title: 'Grüne Grütze', src: 'https://image.livingathome.de/12856600/t/vB/v2/w960/r1/-/lah201210109-kiwi-gruetze-jpg--39250-.jpg', flex: 6 },
      ],
    }),
  }
</script>

<style>
.wrapper{
  margin-top: 60px;
  margin-left: auto;
  margin-right: auto;

}

</style>