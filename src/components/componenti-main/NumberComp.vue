<template>
  <div class="traffic-image py_5">
    <!--inserire contenuto componente-->
    <div class="containers">
        <h6 class="c-blue-lagoon">what are we doing</h6>
        <h2 class="fs-1 fw-bold py-3 text-light"><span class="text-custom">Results</span> in Numbers</h2>
        <div class="box">
            <div v-for="(element, index) in numberUtility" :key="index">
                <span class="c-fountain-blue fw-bold fs-3">{{element.numero}}</span>
                <span class="fw-bold fs-5">{{element.nome}}</span>
            </div>
        </div>
    </div>
    

  </div>
</template>

<script>
export default {
  //Cambiare il nome con quello del componente creato
  name: 'NumberComp',
  data(){
      return{
          numberUtility: [
              {
                  numero: 128,
                  nome: 'Certifications'
              },
              {
                  numero: 230,
                  nome: 'Employees'
              },
              {
                  numero: 517,
                  nome: 'Customers'
              },
              {
                  numero: 94,
                  nome: 'Countries Served'
              },
          ]
      }
  }
    
}
</script>

<style scoped lang="scss">
@import '../../style/variabili.scss';
@import url('https://fonts.googleapis.com/css2?family=Poppins&display=swap');
 /*Inserire style componente*/
 //  utility
.py_5{
     padding: 150px 0;
 }
 .c-silver-sand{
     color: $silver-sand;
 }
 .c-fountain-blue{
     color: $fountain-blue; 
 }
 .c-blue-lagoon{
     color: $blue-lagoon;
 }
// fine utility
 .traffic-image{
     background-image: url(../../assets/img/nextgen.jpg);
     background-size: cover;
 }
 .containers{
     width: 80%;
     margin: 0 auto;
     text-align: center;
     h2{
         padding-top: 20px;
         font-family: 'Poppins', sans-serif;
         font-size: 2.2em;
         color: #fff;
     }
     h6{
     text-transform: uppercase;
     font-size: 0.8em;
    }
 }
 .box{
     display: flex;
     justify-content: space-around;
     div{
         display: flex;
         flex-direction: column;
         color: #fff;
         font-weight: bold;
         font-size: 1.5em;
         margin-top: 50px;
     }
 }
 
 .text-custom{ 
    background-color: $surfiegreen;
    padding: 3px 6px;
    border-radius: 5px;
 }
 
</style>