<template>
  <div class="containers py_5">
    <!--inserire contenuto componente-->
    <div class="box">
        <h6 class="c-blue-lagoon">introduction video</h6>
        <h2>Advisory <span class="text-custom">Perfomance</span> </h2>
        <p class="c-silver-sand">Financial executives nedd to review theri srategies, operating models and capabilities so that their areas cane generate sound information for better decision making.</p>
        <div class="img-video">
            <span><i class="fa-solid fa-play"></i></span>
        </div>
    </div>
    

  </div>
</template>

<script>
export default {
  //Cambiare il nome con quello del componente creato
  name: 'AdvisoryComp',
    
}
</script>

<style scoped lang="scss">
@import '../../style/variabili.scss';
@import url('https://fonts.googleapis.com/css2?family=Poppins&display=swap');

 
 /*Inserire style componente*/
//  utility
.py_5{
     padding: 100px 0;
 }
 .c-silver-sand{
     color: $silver-sand;
 }
 .c-blue-lagoon{
     color: $blue-lagoon;
 }
// fine utility
 .box{
     width: 60%;
     margin: 0 auto;
     text-align: center;
     font-family: Arial, Helvetica, sans-serif;
     h2{
         padding-top: 20px;
         font-family: 'Poppins', sans-serif;
         font-size: 2.2em;
     }
      h6{
     text-transform: uppercase;
     font-size: 0.8em;
    }
    p{
     padding-top: 20px;
     padding-bottom: 40px;
    }
 }
 .containers{
     width: 80%;
     margin: 0 auto;
 }

 .text-custom{
    color: $blue-lagoon; 
    background-color: $tradewind;
    padding: 3px 6px;
    border-radius: 5px;
 }
 
 .img-video{
     background-image: url(../../assets/img/video-1.jpg);
     background-size: cover;
     background-position: center;
     height: 300px;
     display: flex;
     justify-content: center;
     align-items: center;
 }
 .fa-solid{
     font-size: 3.5em;
     text-shadow: 0 -5px $blue-lagoon;
     color: rgba(255, 255, 255, 0.75);
 }
</style>