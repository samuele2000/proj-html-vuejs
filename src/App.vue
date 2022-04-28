<template>
  <div id="app">
    <header>
      <HeaderInfo/>
      <Hero/>    
    </header>
    <main></main>
    <footer></footer>
  </div>
</template>

<script>
  import HeaderInfo from './components/headerComp/HeaderInfo.vue'
  import Hero from './components/headerComp/Hero.vue'

export default {
  name: 'App',
  components: {
    HeaderInfo,
    Hero
  }
}
</script>

<style lang="scss">

</style>
