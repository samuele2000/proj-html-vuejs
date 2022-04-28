<template>
  <div class="dark_blu">
    <!--inserire contenuto componente-->
    <div class="containers d-flex justify-content-between py-3">
      <div>
      <span><i class="fa-solid fa-clock"></i></span>
      <span class="mx-1">Open Hours:</span>
      <span>Mon - Sat 9.00 - 18.00</span>
    </div>
    <div>
      <span><i class="fa-solid fa-phone"></i> +1 (305) 1234-5678</span>
      <span class="mx-3"><i class="fa-solid fa-envelope"></i> hello@example.com</span>
      <a href="#"><i class="fa-brands fa-facebook-f"></i></a>
      <a href="#" class="mx-4"><i class="fa-brands fa-twitter"></i></a>
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
 }
</style>