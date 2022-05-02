<template>
  <div id="app">
    <header>
      <HeaderInfo/>
      <Hero/>  
    </header>

    <main>
      <MainComp/>
    </main>
    
    <footer>
      <FooterLinkComp/>
      <FooterComp2/>
    </footer>
  </div>
</template>

<script>
  import HeaderInfo from './components/componenti-header/HeaderInfo.vue'
  import Hero from './components/componenti-header/Hero.vue'
  import MainComp from './components/MainComp.vue'
  import FooterLinkComp from './components/componenti-footer/FooterLinkComp.vue'
  import FooterComp2 from './components/componenti-footer/FooterComp2.vue'

export default {
  name: 'App',
  components: {
     HeaderInfo, 
     Hero,
    MainComp,
    FooterLinkComp,
    FooterComp2
  }
}
</script>

<style lang="scss">
  // reset
  #app{
    font-family: Arial, Helvetica, sans-serif;
  }
  *{
    padding: 0;
    margin: 0;
    box-sizing: border-box  ;
  }
</style>
