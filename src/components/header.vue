<template>
<div class="border-b-2 p-3 pb-6">
  <div class="flex justify-between">
    <div class="flex">
      <logoheader /><p class="text-xl font-bold text-left text-gray-900 mt-1">Estatery</p>
    </div>
    <div>
      <menu1 />
    </div>
  </div>
</div>
</template>

<script>
import logoheader from "./icones/logo_header.vue"
import menu1 from "./icones/menu.vue"
export default {
  components: { logoheader, menu1 },

        }
</script>