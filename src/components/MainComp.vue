<template>
  <div>
    <!--inserire contenuto componente-->
    <AdvisoryComp/>
    <NumberComp/>
    <!-- <ServicesComp/> -->
    <!-- <TeamComp/>  -->
    <NewsComp/>
    <NewsletterComp/>
    <MessageComp/>
  </div>
</template>

<script>
import AdvisoryComp from './componenti-main/AdvisoryComp.vue'
import NumberComp from './componenti-main/NumberComp.vue'
// import ServicesComp from './componenti-main/ServicesComp.vue'
// import TeamComp from './componenti-main/TeamComp.vue'
import NewsComp from './componenti-main/NewsComp.vue'
import NewsletterComp from './componenti-main/NewsletterComp.vue'
import MessageComp from './componenti-main/MessageComp.vue'
export default {
  //Cambiare il nome con quello del componente creato
  name: 'MainComp',
    components: {
        AdvisoryComp,
         NumberComp,
      //  ServicesComp,
      //  TeamComp,
       NewsComp,
       NewsletterComp,
       MessageComp,
    }
}
</script>

<style scoped lang="scss">
@import '../style/variabili.scss';
 
 /*Inserire style componente*/
 
</style>