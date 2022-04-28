<template>
<div id="hero">
  <div class="d-flex containers justify-content-between py-3 align-items-baseline">
    <LogoComp/>
    <NavComp/>
  </div>
  <div>
    <HeroText/>
  </div>
</div>
  
</template>

<script>
import NavComp from '../partials/NavComp.vue'
import LogoComp from '../partials/LogoComp.vue' 
import HeroText from '../partials/HeroText.vue'
export default {
  //Cambiare il nome con quello del componente creato
  name: 'Hero',
  components: {
    NavComp,
    LogoComp,
    HeroText
  }
}
</script>

<style scoped lang="scss">
@import '../../style/variabili.scss';
 
 /*Inserire style componente*/
  #hero{
    background-image: url(../../assets/img/bg-2.jpg);
    background-position: top;
    background-size: cover;
  }
  .containers{
   width: 80%;
   margin: 0 auto;
 }
</style>