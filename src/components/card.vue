<script>
import bed from './icones/bed.vue'
import bath from './icones/bath.vue'
import size from './icones/size.vue'
import heart from './icones/heart.vue'
export default{
    props:{
        nom: String,
        prix: Number,
        adresse: String,
        favori: Boolean,
        image: String, 
        nbrSDB: Number,
        nbrBED: Number,
        nbrAREA: Number
    },
    components: { bed, bath, size, heart }
}
</script>
<template>
    <figure>
        <img class="rounded-t-lg" :src="image" alt="" />
    <figcaption class="flex flex-col relative rouned-b-lg border-2 border-t-0 px-5 py-7">
        <h3 class="text-2xl text-gray-900">{{nom}}</h3>
        <address class="not-italic text-gray-500">{{adresse}}</address>
        <div class="flex items-center order-first">
            <div class="text-2xl text-indigo-500">${{prix}}</div>
            <div class="text-gray-500">/mois</div>
        </div>
        <hr class="my-2 border-indigo-100 border-t-2"/>
        <div class="flex justify-between text-sm">
            <div><bed class="inline-block align-top"/>{{nbrBED}} Beds</div>
            <div><bath class="inline-block align-top"/>{{nbrSDB}} Bathrooms</div>
            <div><size class="inline-block align-top"/>{{nbrAREA}} m²</div>
        </div>
        <div class='w-12 h-12 border-2 border-indigo-100 rounded-full absolute top-7 right-5 grid place-items-center'>
            <heart :class="{'fill-red-300': favori}" />
        </div>
    </figcaption>
    </figure>
</template>
