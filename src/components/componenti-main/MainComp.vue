<template>
  <div>
    <!--inserire contenuto componente-->
    <AdvisoryComp />
    <NumberComp />
    <ServicesComp />
    <TeamComp />
    <NewsComp />
    <NewsletterComp />
    <MessageComp />
  </div>
</template>

<script>
  import AdvisoryComp from './AdvisoryComp.vue'
  import NumberComp from './NumberComp.vue'
  import ServicesComp from './ServicesComp.vue'
  import TeamComp from './TeamComp.vue'
  import NewsComp from './NewsComp.vue'
  import NewsletterComp from './NewsletterComp.vue'
  import MessageComp from './MessageComp.vue'
  export default {
    //Cambiare il nome con quello del componente creato
    name: 'MainComp',
    components: {
      AdvisoryComp,
      NumberComp,
      ServicesComp,
      TeamComp,
      NewsComp,
      NewsletterComp,
      MessageComp,
    }
  }
</script>

<style scoped lang="scss">
  @import '../../style/variabili.scss';

  /*Inserire style componente*/
</style>