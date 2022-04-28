<template>
  <div>
    <!--inserire contenuto componente-->
    <AdvisoryComp/>
    

  </div>
</template>

<script>
import AdvisoryComp from './componenti-main/AdvisoryComp.vue'
export default {
  //Cambiare il nome con quello del componente creato
  name: 'MainComp',
    components: {
       AdvisoryComp 
    }
}
</script>

<style scoped lang="scss">
@import '../style/variabili.scss';
 
 /*Inserire style componente*/
 
</style>