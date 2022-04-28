<template>
  <div class="traffic-image py_5">
    <!--inserire contenuto componente-->
    <div class="containers text-center">
        <h6 class="text-uppercase">what are we doing</h6>
        <h2 class="fs-1 fw-bold py-3 text-light"><span class="text-custom">Results</span> in Numbers</h2>
        <div class=" d-flex justify-content-between">
            <div v-for="(element, index) in numberUtility" :key="index" class="text-light d-flex flex-column mt-5">
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
                  nome: 'Employes'
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
 
 /*Inserire style componente*/
 .traffic-image{
     background-image: url(../../assets/img/bg-1.jpg);
 }
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
 .text-custom{ 
    background-color: $tradewind;
    padding: 3px 6px;
    border-radius: 5px;
 }
 .py_5{
     padding: 100px 0;
 }
 .c-fountain-blue{
     color: $fountain-blue; 
 }
</style>