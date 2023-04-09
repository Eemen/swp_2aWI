
<template>
  <v-app class="bgcolor">
    <v-navigation-drawer v-model="drawer" app class="nav-drawer"
        image="https://www.colorhexa.com/fff0db.png"> 
      <v-list class="sliderclass">
        <v-list-item class="sliderclass"
          prepend-avatar="https://randomuser.me/api/portraits/women/85.jpg"
          title="Sandra Adams"
          subtitle="sandra_a88@gmailcom"
        ></v-list-item>
      </v-list>

      <v-divider class="sliderclass"></v-divider>

      <v-list dense nav >
        <v-list-item class="sliderclass" ><v-text-field
          hide-details prepend-icon="mdi-magnify"
        ></v-text-field></v-list-item>
        <v-list-item class="sliderclass" ><v-btn prepend-icon="mdi-star" color="#e6d2b8" @click="scrollTofav">Top Rezepte</v-btn></v-list-item>
        <v-list-item class="sliderclass" ><v-btn prepend-icon="mdi-star" color="#e6d2b8" @click="scrollToTag">Unser Tages Menü</v-btn></v-list-item>
      </v-list>
    </v-navigation-drawer>

    <v-app-bar app>
      <v-app-bar-nav-icon @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
    </v-app-bar>
    <v-main>
    <VCard class="sliderflex">
      <VCard width="100%">

          <p class="namediv">Kochrezepte.at</p>
        
         <v-carousel hide-delimiters class="itemdiv"> 

          <v-carousel-item
                src="https://www.einfachbacken.de/sites/einfachbacken.de/files/styles/full_width_tablet_4_3/public/2019-08/kaiserschmarrn.jpg?h=a1e1a043&itok=CHvFnq-t"
                cover
              >
              <div class="essendiv">      
                  <h1>
                    Kaiserschmarrn
                  </h1>
                </div>  </v-carousel-item>
            
              <v-carousel-item
                src="https://www.gusto.at/_storage/asset/12423448/storage/womanat:slideshow-large/file/177956045/83509600.jpg"
                cover>

              
              <div class="essendiv">      
                  <h1>
                    Frühlingsrollen
                  </h1>
                </div>  
              </v-carousel-item>

              <v-carousel-item
                src="https://www.gutekueche.at/storage/media/recipe/106126/conv/wiener-schnitzel-default.jpg"
                cover>
                <div class="essendiv">      
                  <h1>
                     Wiener Schnitzel
                  </h1>
                </div>  
            </v-carousel-item>

              <v-carousel-item
                src="https://www.daskochrezept.de/sites/daskochrezept.de/files/styles/full_width_tablet_4_3/public/2022-01/2022_palatschinken_aufmacher.jpg?h=4a175897&itok=javqpYmI"
                cover
              >
              <div class="essendiv">      
                  <h1>
                    Palatschinken
                  </h1>
                </div>  </v-carousel-item>

              <v-carousel-item
                src="https://cdn.gutekueche.de/upload/rezept/4070/1600x1200_glutenfreie-schokoladen-kekse.jpg"
                cover
              >
              <div class="essendiv">      
                  <h1>
                    Schoko Kekse
                  </h1>
                </div>  </v-carousel-item>

            </v-carousel>
        </VCard>
      </VCard>
    </v-main>
  </v-app>
  </template>
  
  



  <script>
  
  export default {
    data() {
      return {
        drawer: false,
        items: [
          { icon: 'mdi-folder', title: 'My Files', route: '#' },
          { icon: 'mdi-account-multiple', title: 'Shared with me', route: '/shared' },
          { icon: 'mdi-star', title: 'Starred', route: '/starred' },
        ],
        colors: [
        'indigo',
        'warning',
        'pink darken-2',
        'red lighten-1',
        'deep-purple accent-4',
        ],
        slides: [
        'Bild',
        'Second',
        'Third',
        'Fourth',
        'Fifth',
      ],
      };
    },
    methods: {
  scrollTofav() {
    document.getElementById("fav").scrollIntoView({behavior: "smooth"})
  },
  scrollToTag() {
    document.getElementById("tag").scrollIntoView({behavior: "smooth"})
  }
}

  };
  

  </script>

<style>
.sliderclass{
  border-color: white;
  background-color:	#fff0db;
}

.sliderflex{
  display: flex;
  align-items: center;
  justify-content: center;
  border-color: white;
  border: none;
  background-color:	#fff0db;
}

.bgcolor{
  background-color: #fff0db;
  border-color: none;
  height:50%;
}

.nav-drawer{
  z-index: 10000;
}

.essendiv{
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100%;
  width: 100%;
  color: white;
  font-family: 'Alkatra', cursive;
}

.essendiv:hover{
  text-decoration: underline
}

@import url('https://fonts.googleapis.com/css2?family=Alkatra&display=swap');

.namediv{
  z-index: 10000;
  margin-top: 0px;
  text-align: center;
  background-color: #fff0db;
  width: 100%;
  color: black;
  font-family: 'Alkatra', cursive;
  font-size: 40px;
  position: absolute;
}

.itemdiv{
  z-index: 90;
}
</style>