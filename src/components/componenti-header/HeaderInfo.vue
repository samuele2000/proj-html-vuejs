<template>
  <div class="dark_blu">
    <!--inserire contenuto componente-->
    <div class="containers">
      <div>
      <span><i class="fa-solid fa-clock"></i></span>
      <span class="mx-10">Open Hours:</span>
      <span>Mon - Sat</span>
      <span class="mx-10">9.00 - 18.00</span>
    </div>
    <div>
      <span><i class="fa-solid fa-phone"></i> +1 (305) 1234-5678</span>
      <span class="mx-15"><i class="fa-solid fa-envelope"></i> hello@example.com</span>
      <a href="#"><i class="fa-brands fa-facebook-f"></i></a>
      <a href="#" class="mx-20"><i class="fa-brands fa-twitter"></i></a>
      <a href="#"><i class="fa-brands fa-linkedin-in"></i></a>
    </div>
  </div>
    

  </div>
</template>

<script>
export default {
  //Cambiare il nome con quello del componente creato
  name: 'HeaderInfo',

}
</script>

<style scoped lang="scss">
@import '../../style/variabili.scss';
 
 /*Inserire style componente*/
//  utility
.mx-10{
  margin: 0 10px;
}
.mx-15{
  margin: 0 15px;
}
.mx-20{
  margin: 0 20px;
}
// fine utility 
 div{
   color: $silver-sand;
 }
 a{
   color: $silver-sand;
 }
 .dark_blu{
   background-color: $dark-blu;
 }
 .containers{
   width: 80%;
   margin: 0 auto;
   display: flex;
   justify-content: space-between;
   padding: 14px 0;
   font-size: 0.8em;
 }
</style>