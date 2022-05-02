<template>
<div id="hero">
  <div class="containers">
    <LogoComp/>
    <NavComp/>
  </div>
  <HeroText class="heroText"/>
 
</div>
  
</template>

<script>
import NavComp from './NavComp.vue'
import LogoComp from './LogoComp.vue' 
import HeroText from './componenti-hero/HeroText.vue'
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
    background-position: center;
    background-size: cover;
    height: 700px;
    position: relative;
  }
  .containers{
   width: 80%;
   margin: 0 auto;
   display: flex;
   justify-content: space-between;
   padding-top: 20px;
   align-items: baseline;
 }
  .heroText{
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100%;
  }
</style>