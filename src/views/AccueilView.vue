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
</template>

<script>
import IconeMenu from "../components/icons/IconeMenu.vue";
import IconeLogoSite from "../components/icons/IconeLogoSite.vue";
import LoginButton from "../components/buttons/LoginButton.vue";
import FlecheMenu from "../components/FlecheMenu.vue"

export default {
  components: {
    IconeMenu,
    IconeLogoSite,
    LoginButton,
    FlecheMenu,
  },
};
</script>