<template>
  <div class="bg_color">
    <!--inserire contenuto componente-->
    <div class="containers">
      <div>
      <span class="">Enjoy the low price. We are tracking any intention of privacy.</span>
    </div>
    <div>
      <span><i class="fa-regular fa-copyright"></i> 2020 NEXGEN is Proudly Powered by <span class="c-blue-lagoon">Codings</span></span>
    </div>
  </div>
    

  </div>
</template>

<script>
export default {
  //Cambiare il nome con quello del componente creato
  name: 'FooterComp2',

}
</script>

<style scoped lang="scss">
@import '../../style/variabili.scss';
 
 /*Inserire style componente*/
 .c-blue-lagoon {
        color: $blue-lagoon;
    }
 div{
   color: $silver-sand;
   font-size: 0.9em;
 }
 .bg_color{
   background-color: $woodsmoke;
 }
 .containers{
   width: 80%;
   margin: 0 auto;
   display: flex;
   justify-content: space-between;
   padding: 20px 0;
 }
</style>