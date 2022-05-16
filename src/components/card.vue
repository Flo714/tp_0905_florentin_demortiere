<template>
    <figure class="m-4">
        <img class="rounded-t-lg" :src="image" alt="">
        <figcaption class="flex flex-col relative px-5 py-7 border-2 border-t-0 rounded-b-lg">
            <h3 class="text-2xl text-gray-900">{{nom}}</h3>
           <address class="not-italic text-gray-500">{{texte}}</address> 
           <div class="order-first flex items-center">
               <div class="text-2xl text-indigo-500">${{price.toLocaleString("en-US")}}</div>
               <div class="text-gray-500">/mois</div>
           </div>
            <hr class="border-indigo-100 border-t-2 my-2"/>
            <div class="flex justify-between text-sm">
                <div><bed class="inline-block align-top"/> 4 Beds</div>
                <div><bath class="inline-block align-top"/>{{bathroom}}</div>
                <div><size class="inline-block align-top"/>{{size}}</div>
            </div>
            <div class="grid place-items-center w-12 h-12 border-2 border-indigo-100 rounded-full absolute top-7 right-4">
                <heart :class="{ 'fill-red-400': favoris}"/>
            </div>
        </figcaption>
    </figure>
</template>

<script>
    import bed from "./icones/bed.vue"
    import bath from "./icones/bath.vue"
    import size from "./icones/size.vue"
    import heart from "./icones/hearth.vue"
    export default {
        props: {
            price: {
                type: Number, 
                default: 2700
            }, 
            favoris:{
                type: Boolean,
                default: false,
            },
            nom : {
                type: String,
                default: "Beverly Springfield",
            },
            texte : {
                type: String,
                default: "2821 Lake Sevilla, Palm Harbor, TX",
            },
            image : {
                type: String,
            },
            bathroom: {
                type: String,
                default: "2 Bathrooms",
            },
            size: {
                type: String,
                default: "6x7.5 m²",
            },
        },
        components: { bed, bath, size, heart}
    }
</script>