<template>
  <div class="containers text-center pb_5">
      <div class="box">
        <h2 class="text-white fw-bold fs-1">Financial Risk</h2>  
        <p class="py-3">
            The right outcomes depend on continuous rigor in governance, models, and
            processes across the finance function.
        </p>
        <button type="button" class="btn text-uppercase button_color text-light fw-bold">get in touch</button>
        <button type="button" class="btn text-uppercase text-light fw-bold ms-3 border-blue-lagoon px-3">read more</button>
      </div>   
  </div>
</template>

<script>
export default {
  //Cambiare il nome con quello del componente creato
  name: 'HeroText',
  

}
</script>

<style scoped lang="scss">
@import '../../style/variabili.scss';
 
 /*Inserire style componente*/
.button_color{
     background-color: $blue-lagoon;
 }
 .box{
     width: 50%;
     margin: 100px auto;
 }
 p{
     color: $silver-sand;
 }
 .pb_5{
     padding-bottom: 100px;
 }
 .border-blue-lagoon{
   border: 1px solid $blue-lagoon;
 }
</style>