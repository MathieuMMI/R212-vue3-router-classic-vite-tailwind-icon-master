<template>
  <div class="flex justify-between items-center self-stretch flex-grow-0 flex-shrink-0 h-[66px] relative bg-white/40 border border-[#f6f8ff] backdrop-blur-[80px]">
  <div class="flex justify-start items-center flex-grow-0 flex-shrink-0 gap-12">
    <div class="flex justify-start items-start flex-grow-0 flex-shrink-0 w-[151px] relative overflow-hidden gap-8">
      <div class="flex-grow-0 flex-shrink-0 w-[151px] h-10 relative overflow-hidden">
        <p class="absolute left-11 top-[9px] text-xl font-bold text-left text-gray-900">Estatery</p>
      </div>
    </div>
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

export default {
  components: {
    IconeMenu,
    IconeLogoSite,
    LoginButton,
  },
};
</script>