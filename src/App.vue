<template>
  <div id="app">
    <header>
      <HeaderInfo/>
      <Hero/>    
    </header>

    <main>
      <MainComp/>
    </main>
    
    <footer></footer>
  </div>
</template>

<script>
  import HeaderInfo from './components/headerComp/HeaderInfo.vue'
  import Hero from './components/headerComp/Hero.vue'
  import MainComp from './components/MainComp.vue'

export default {
  name: 'App',
  components: {
    HeaderInfo,
    Hero,
    MainComp
  }
}
</script>

<style lang="scss">

</style>
