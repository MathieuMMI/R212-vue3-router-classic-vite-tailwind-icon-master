<template>
  <div class="flex justify-between items-center self-stretch flex-grow-0 flex-shrink-0 h-[66px] relative bg-white/40 border border-[#f6f8ff] backdrop-blur-[80px]">
  <div class="flex justify-start items-center flex-grow-0 flex-shrink-0 gap-12">
    <div class="flex justify-start items-start flex-grow-0 flex-shrink-0 w-[151px] relative overflow-hidden gap-8">
      <div class="flex-grow-0 flex-shrink-0 w-[151px] h-10 relative overflow-hidden">
        <p class="absolute left-11 top-[9px] text-xl font-bold text-left text-gray-900">Estatery</p>
      </div>
    </div>
  </div>
  <div class="hidden xl:flex items-center overflow-hidden relative gap-2.5">
    <div class="flex overflow-hidden gap-10">
      <p class="flex-grow-0 flex-shrink-0 text-base font-medium text-left text-gray-900">Rent</p>
      <p class="flex-grow-0 flex-shrink-0 text-base font-medium text-left text-gray-900">Buy</p>
      <p class="flex-grow-0 flex-shrink-0 text-base font-medium text-left text-gray-900">Sell</p>
      <p class="flex-grow-0 flex-shrink-0 text-base font-medium text-left text-gray-900">Manage Property</p>
    </div>
    <fleche-menu/>
    <div class="flex justify-start items-center overflow-hidden gap-10">
      <p class="flex-grow-0 flex-shrink-0 text-base font-medium text-left text-gray-900">Resources</p>
    </div>
    <fleche-menu/>
  </div>

<login-button />  
<icone-logo-site />
<icone-menu class="xl:hidden" />
</div>
<div class="p-2  grid grid-flow-row-dense grid-cols-[repeat(auto-fit,minmax(100px,1fr))]">
  <card 
    :prix= "2700"
    :favori= "false" 
    :nbr-s-d-b= "2" 
    :nbr-b-e-d= "6" 
    :nbr-a-r-e-a= "100" 
    nom= "Beverly Springfield" 
    adresse= "2821 Lake Sevilla, Palm Harbor, TX" 
    image= "/images-maisons/maison-1.jpg"/>
  <card 
    :prix= "2095"
    :favori= "false" 
    :nbr-s-d-b= "3" 
    :nbr-b-e-d= "5" 
    :nbr-a-r-e-a= "90" 
    nom= "Palm Harbor" 
    adresse= "2699 Green Valley, Highland Lake" 
    image= "/images-maisons/maison-2.jpg"/>
  <card 
    :prix= "4550"
    :favori= "false" 
    :nbr-s-d-b= "1" 
    :nbr-b-e-d= "4" 
    :nbr-a-r-e-a= "250" 
    nom= "Faulkner Ave" 
    adresse= "909 Woodland St, Michigan, IN" 
    image= "/images-maisons/maison-3.jpg"/>
  <card 
    :prix= "4650"
    :favori= "true" 
    :nbr-s-d-b= "4" 
    :nbr-b-e-d= "3" 
    :nbr-a-r-e-a= "300" 
    nom= "St. Christal" 
    adresse= "210 US Highway, HighlandLake, FL" 
    image= "/images-maisons/maison-4.jpg"/>
  <card 
    :prix= "3100"
    :favori= "false" 
    :nbr-s-d-b= "1" 
    :nbr-b-e-d= "2" 
    :nbr-a-r-e-a= "70" 
    nom= "Cover Red" 
    adresse= "243 CurlewRoad, PalmHarbor, TX" 
    image= "/images-maisons/maison-5.jpg"/>
      <card 
    :prix= "4800"
    :favori= "true" 
    :nbr-s-d-b= "2" 
    :nbr-b-e-d= "7" 
    :nbr-a-r-e-a= "350" 
    nom= "Tarpon Bay" 
    adresse= "103 Lake Shores, Michigan, IN" 
    image= "/images-maisons/maison-6.jpg"/>
</div>
</template>

<script>
import IconeMenu from "../components/icons/IconeMenu.vue";
import IconeLogoSite from "../components/icons/IconeLogoSite.vue";
import LoginButton from "../components/buttons/LoginButton.vue";
import FlecheMenu from "../components/FlecheMenu.vue"
import color from '../components/color.vue'
import card from '../components/card.vue'

export default {
  components: {
    IconeMenu,
    IconeLogoSite,
    LoginButton,
    FlecheMenu,
    color, 
    card,
  },
};
</script>