<template>
  <div>
      <div class="box">
        <h2 class="f-family">Financial Risk</h2>  
        <p class="py-3">
            The right outcomes depend on continuous rigor in governance, models, and
            processes across the finance function.
        </p>
        <button type="button" class="button-all button_color">get in touch</button>
        <button type="button" class="button-empty">read more</button>
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
@import '../../../style/variabili.scss';
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@800&display=swap');
 
 /*Inserire style componente*/
//  utility
  .button-all {
        text-transform: uppercase;
        color: #fff;
        padding: 10px 15px;
        border-radius: 5px;
        border: none;
        margin-right: 20px;
    }
    .button-all:hover {
        background-color: $fountain-blue;
    }
    .button-empty {
        background-color: transparent;
        border: 1px solid $blue-lagoon;
        text-transform: uppercase;
        color: #fff;
        padding: 10px 20px;
        border-radius: 5px;
        margin-top: 20px;
    }
    .button-empty:hover {
        background-color: $fountain-blue;
        border-color: $fountain-blue;
        color: #fff;
    }
    .button_color{
     background-color: $blue-lagoon;
 }
 .f-family{
   font-family: 'Poppins', sans-serif;
 }
// fine utility


 .box{
     width: 40%;
     text-align: center;
     font-family:Arial, Helvetica, sans-serif;
     h2{
       color: #fff;
       font-weight: bold;
       font-size: 3em;
     }
 }
 p{
     color: $silver-sand;
     padding: 15px 0;
     font-size: 1.1em;
 }

</style>