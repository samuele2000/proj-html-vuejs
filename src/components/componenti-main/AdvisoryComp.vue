<template>
  <div class="containers text-center py_5">
    <!--inserire contenuto componente-->
    <div class="box">
        <h6 class="text-uppercase">introduction video</h6>
        <h2 class="fs-1 fw-bold py-3">Advisory <span class="text-custom">Perfomance</span> </h2>
        <p>Financial executives nedd to review theri srategies, operating models and capabilities so that their areas cane generate sound information for better decision making.</p>
        <div class="img-video d-flex align-items-center justify-content-center">
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
 
 /*Inserire style componente*/
 .box{
     width: 60%;
     margin: 0 auto;
 }
 .containers{
     width: 80%;
     margin: 0 auto;
 }
 h6{
     color: $blue-lagoon;
 }
 p{
     color: $silver-sand;
 }
 .text-custom{
    color: $blue-lagoon; 
    background-color: $tradewind;
    padding: 3px 6px;
    border-radius: 5px;
 }
 .py_5{
     padding: 100px 0;
 }
 .img-video{
     background-image: url(../../assets/img/video-1.jpg);
     background-size: cover;
     background-position: center;
     height: 300px;
 }
 .fa-solid{
     font-size: 3.5em;
     text-shadow: 0 -5px $blue-lagoon;
     color: rgba(255, 255, 255, 0.75);
 }
</style>