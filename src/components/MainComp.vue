<template>
  <div>
    <!--inserire contenuto componente-->
    <AdvisoryComp/>
    <NumberComp/>
    <ServicesComp/>

  </div>
</template>

<script>
import AdvisoryComp from './componenti-main/AdvisoryComp.vue'
import NumberComp from './componenti-main/NumberComp.vue'
import ServicesComp from './componenti-main/ServicesComp.vue'
export default {
  //Cambiare il nome con quello del componente creato
  name: 'MainComp',
    components: {
       AdvisoryComp,
       NumberComp,
       ServicesComp,
    }
}
</script>

<style scoped lang="scss">
@import '../style/variabili.scss';
 
 /*Inserire style componente*/
 
</style>