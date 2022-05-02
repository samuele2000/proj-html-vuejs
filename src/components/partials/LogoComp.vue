<template>
  <div>
      <h2><span class="nex-custom">nex</span><span class="gen-custom">gen</span></h2>
  </div>
</template>

<script>
export default {
  //Cambiare il nome con quello del componente creato
  name: 'LogoComp',
  

}
</script>

<style scoped lang="scss">
@import '../../style/variabili.scss';
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@700&display=swap');
 
 /*Inserire style componente*/
 h2{
   text-transform: uppercase ;
   font-family: 'Montserrat', sans-serif;
   font-size: 1.1em;
   font-weight: 900;
   letter-spacing: 5px;
 }
 .nex-custom{
   color: $blue-lagoon;
   background-color: $surfiegreen;
   padding: 7px 0px 7px 20px;
   border-radius: 50px 0 0 50px;  
 }
 .gen-custom{
   color: $silver-sand;
   margin-left: 3px;
 }
 
</style>