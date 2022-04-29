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
  import HeaderInfo from './components/headerComp/HeaderInfo.vue'
  import Hero from './components/headerComp/Hero.vue'
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

</style>
