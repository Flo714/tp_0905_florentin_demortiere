<template>
  <div class="bg-indigo-25">
    <div>
      <header1 />
    </div>

    <div class="lg:flex lg:justify-between">
      <h1 class="m-4 mt-14 text-4xl font-bold text-center">Search properties to rent</h1>

      <div class="mt-14 mx-6 px-2 border-2 border-indigo-100 rounded-lg flex justify-between bg-white lg:flex-1 lg:ml-48 lg:pt-2 lg:pb-2">
          <p class="text-gray-900 font-medium text-left pt-1 lg:">Search with Search Bar</p>

          <flechebas class="p-2 my-1 bg-indigo-100 rounded-xl "/>
      </div>
    </div>

    <div class="mt-10 mx-6 flex justify-between bg-white rounded-lg">
      <p class=" px-2 py-4 text-gray-500 font-medium">Search location</p>

      <search class="bg-indigo-500 m-2 p-3"/>
    </div>


    <div class="mt-4 p-2 grid grid-flow-row-dense grid-cols-[repeat(auto-fit,minmax(300px,1fr))]">
      <card :price="2700" nom="Beverly Springfield" texte="2821 Lake Sevilla, Palm Harbor, TX" image="/public/image/pexels-binyamin-mellish-106399 1.png" bathroom="2 Bathrooms" size="6x7.5 m²"/>
      <card :price="4800" nom="Tarpon Bay" texte="103 Lake Shores, Michigan, IN" image="/public/image/pexels-binyamin-mellish-106399_2.png" bathroom="2 Bathrooms" size="6x7.5 m²"/>
      <card :price="2095" nom="Palm Harbor" texte="2699 Green Valley, Highland Lake" image="/public/image/pexels-binyamin-mellish-106399 4.png" bathroom="2 Bathrooms" size="6x7 m²"/>
      <card :price="4550" nom="Faulkner Ave" texte="909 Woodland St, Michigan, IN" image="/public/image/pexels-binyamin-mellish-106399 3.png" bathroom="3 Bathrooms" size="8x10 m²"/>
      <card :price="4650" nom="St. Christal" texte="210 US Highway, HighlandLake, FL" image="/public/image/pexels-binyamin-mellish-106399 5.png" bathroom="2 Bathrooms" size="6x7.5 m²"/>
      <card :price="3100" nom="Cover Red" texte="243 CurlewRoad, PalmHarbor, TX" image="/public/image/pexels-binyamin-mellish-106399 6.png" bathroom="2 Bathrooms" size="6x7.5 m²"/>
    </div>
  </div>
  <div>
    <footer1 />
  </div>


</template>
<script>
import card from "./components/card.vue"
import { FilmIcon, MenuIcon, DownloadIcon  } from "@heroicons/vue/solid";
import { initCustomFormatter } from '@vue/runtime-core';
import header1 from './components/header.vue';
import footer1 from './components/footer.vue';
import flechebas from './components/icones/flechebas.vue'
import search from './components/icones/search.vue'
export default {
  name: "App",
  components:  { card, header1, footer1, flechebas, search}
};
</script>