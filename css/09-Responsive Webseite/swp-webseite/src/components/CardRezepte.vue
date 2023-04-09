<template>
    <p class="favuberschrift" id="fav">Unsere Top Rezepte</p>
    <div class="wrapper-flex">
        
        <v-card
        class="mx-auto"
        max-width="344"
        >
        <v-img
            src="https://www.gutekueche.at/storage/media/recipe-category/7545/conv/gugelhupf-rezepte-default.jpg"
            height="200px"
            cover
        ></v-img>
    
        <v-card-title>
            Marmorgugelhupf
        </v-card-title>
    
        <v-card-subtitle>
            <v-rating
             v-model="rating"
            hover
            half-increments
            color="yellow"
            model-value="5"
             ></v-rating>
        </v-card-subtitle>
    
        <v-card-actions>
            <v-btn
            color="orange-lighten-2"
            variant="text"
            >
            Zubereitung
            </v-btn>
    
            
            <v-spacer></v-spacer>
    
            <v-btn
            :icon="show ? 'mdi-chevron-up' : 'mdi-chevron-down'"
            @click="show = !show"
            ></v-btn>
        </v-card-actions>
    
        <v-expand-transition>
            <div v-show="show">
            <v-divider></v-divider>
    
            <v-card-text>
                Ein Gugelhupf hat viele gute Eigenschaften. Zum einen ist er sehr vielseitig und kann mit unterschiedlichen Zutaten und Aromen zubereitet werden. Er ist ein Klassiker unter den Kuchen und eignet sich perfekt für gemütliche Kaffeekränzchen. Außerdem bleibt er durch seine besondere Form lange frisch und saftig. Durch seine lockere Konsistenz und den feinen Geschmack ist er auch bei Kindern sehr beliebt. Zusammenfassend lässt sich sagen, dass ein Gugelhupf ein leckeres und traditionelles Gebäck ist, das bei vielen Gelegenheiten für Freude sorgt.
            </v-card-text>
            </div>
        </v-expand-transition>
        </v-card>

        <v-card
        class="mx-auto"
        max-width="344"
        >
        <v-img
            src="https://www.einfachbacken.de/sites/einfachbacken.de/files/styles/full_width_tablet_4_3/public/2020-03/klassischer_kasekuchen_2.jpg?h=4521fff0&itok=-W9far_5"
            height="200px"
            cover
        ></v-img>
    
        <v-card-title>
            Käsekuchen
        </v-card-title>
    
        <v-card-subtitle>
            <v-rating 
             v-model="rating"
            hover
            half-increments
            color="yellow"
            model-value="5"
             ></v-rating>
        </v-card-subtitle>
    
        <v-card-actions>
            <v-btn
            color="orange-lighten-2"
            variant="text"
            >
            Zubereitung
            </v-btn>
    
            <v-spacer></v-spacer>
    
            <v-btn
            :icon="show ? 'mdi-chevron-up' : 'mdi-chevron-down'"
            @click="show = !show"
            ></v-btn>
        </v-card-actions>
    
        <v-expand-transition>
            <div v-show="show">
            <v-divider></v-divider>
    
            <v-card-text>
                Ein klassischer Käsekuchen hat viele Vorzüge. Der cremige und sahnige Geschmack des Kuchens ist unvergleichlich. Der Käsekuchen eignet sich perfekt für viele Anlässe, ob als Dessert oder als Geburtstagskuchen. Er ist auch bei Menschen mit einer Vorliebe für süße und herzhafte Gerichte gleichermaßen beliebt. Der Käsekuchen hat eine besondere Konsistenz, die ihn so unwiderstehlich macht. Er bleibt auch nach einigen Tagen noch frisch und lecker. Zusammenfassend lässt sich sagen, dass ein klassischer Käsekuchen ein echter Allrounder unter den Kuchen ist, der jeden Gaumen begeistert.
            </v-card-text>
            </div>
        </v-expand-transition>
        </v-card>

        <v-card
        class="mx-auto"
        max-width="344"
        >
        <v-img
            src="https://backen.de/backen.de/Recipes/e/Einfacher-apfelkuchen/Beauties%20neu/Einfacher-Apfelkuchen_Eyelevel_neu.jpg"
            height="200px"
            cover
        ></v-img>
    
        <v-card-title>
            Apfelkuche
        </v-card-title>
    
        <v-card-subtitle>
            <v-rating
             v-model="rating"
            hover
            half-increments
            color="yellow"
            model-value="5"
             ></v-rating>
        </v-card-subtitle>
    
        <v-card-actions>
            <v-btn
            color="orange-lighten-2"
            variant="text"
            >
            Zubereitung
            </v-btn>
    
            <v-spacer></v-spacer>
    
            <v-btn
            :icon="show ? 'mdi-chevron-up' : 'mdi-chevron-down'"
            @click="show = !show"
            ></v-btn>
        </v-card-actions>
    
        <v-expand-transition>
            <div v-show="show">
            <v-divider></v-divider>
    
            <v-card-text>
                Ein einfacher Apfelkuchen hat viele Vorzüge. Der fruchtige und erfrischende Geschmack des Kuchens ist unverwechselbar. Der Apfelkuchen ist ein Klassiker unter den Kuchen und eignet sich perfekt für gemütliche Kaffeekränzchen oder als Snack zwischendurch. Die Kombination aus saftigen Äpfeln und knusprigem Teig macht ihn zu einem echten Gaumenschmaus. Durch seine einfache Zubereitung ist er auch bei Hobbybäckern sehr beliebt. Zusammenfassend lässt sich sagen, dass ein einfacher Apfelkuchen ein leckeres und traditionelles Gebäck ist, das bei vielen Gelegenheiten für Genuss sorgt.
            </v-card-text>
            </div>
        </v-expand-transition>
        </v-card>

        <v-card
        class="mx-auto"
        max-width="344"
        >
        <v-img
            src="https://www.daskochrezept.de/sites/daskochrezept.de/files/styles/full_width_tablet_4_3/public/2021-07/erdbeerkuchen_mit_vanillepudding_21.jpg?h=4521fff0&itok=FFN-x69f"
            height="200px"
            cover
        ></v-img>
    
        <v-card-title>
            Erdbeerkuchen
        </v-card-title>
    
        <v-card-subtitle>
            <v-rating
             v-model="rating"
            hover
            half-increments
            color="yellow"
            model-value="5"
             ></v-rating>
        </v-card-subtitle>
    
        <v-card-actions>
            <v-btn
            color="orange-lighten-2"
            variant="text"
            >
            Zubereitung
            </v-btn>
    
            <v-spacer></v-spacer>
    
            <v-btn
            :icon="show ? 'mdi-chevron-up' : 'mdi-chevron-down'"
            @click="show = !show"
            ></v-btn>
        </v-card-actions>
    
        <v-expand-transition>
            <div v-show="show">
            <v-divider></v-divider>
    
            <v-card-text>
                Ein Erdbeerkuchen mit Vanillepudding hat viele Vorzüge. Der fruchtige Geschmack der Erdbeeren harmoniert perfekt mit der sanften Süße des Vanillepuddings. Der Erdbeerkuchen ist ein beliebtes Gebäck, das vor allem in den Sommermonaten gerne gegessen wird. Er eignet sich perfekt für Gartenpartys oder Picknicks im Grünen. Durch die frischen Zutaten und die leichte Zubereitung ist er auch bei gesundheitsbewussten Menschen sehr beliebt. Zusammenfassend lässt sich sagen, dass ein Erdbeerkuchen mit Vanillepudding ein fruchtiges und erfrischendes Gebäck ist, das bei vielen Gelegenheiten für Genuss sorgt.
            </v-card-text>
            </div>
        </v-expand-transition>
        </v-card>

    </div>
</template>

  
<script>
export default {
  data: () => ({
    show: true,
  }),
}

</script>

<style>


.wrapper-flex {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  background-color: #fff0db;
}

.mx-auto{
    width: 344px;
}

.favuberschrift{
  width: 100%;
  color: black;
  font-family: 'Alkatra', cursive;
  text-align: center;
  font-size: 35px;
  background-color: #fff0db;
  padding-bottom: 30px;

}

.wrapper-flex .v-card{
    margin-top: 20px;
}



</style>


