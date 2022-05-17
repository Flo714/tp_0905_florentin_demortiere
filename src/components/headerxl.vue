<template>
<div class="border-b-2 p-3 pb-6">
  <div class="flex">
    <div class="flex">
      <logoheader /><p class="text-xl font-bold text-left text-gray-900 mt-1">Estatery</p>
    </div>
    <div class="flex">
        <p class="m-2">Rent</p>
        <p class="m-2">Buy</p>
        <p class="m-2">Sell</p>
        <div class="flex">
          <p class="m-2">Manage Property</p>
        <flechebas />
          </div>

      <div class="flex">
        <p class="m-2">Ressources</p>
        <flechebas />
      </div>
    </div>
    <div class="flex">
      <p class="bg-white text-indigo-500 border-2 border-indigo-200 px-4 py-2 rounded-lg m-2 text-center">Login</p>
      <p class="bg-indigo-500 text-white px-5 py-2 rounded-lg m-2 text-center">Sign up</p>
    </div>
  </div>
</div>
</template>

<script>
import logoheader from "./icones/logo_header.vue"
import menu1 from "./icones/menu.vue"
import flechebas from "./icones/flechebas.vue"
export default {
  components: { logoheader, menu1, flechebas },

        }
</script>