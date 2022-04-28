<template>
  <div class="d-flex align-items-baseline">
      <ul class="d-flex">
          <li v-for="(element, index) in menuNav" :key="(index)" class="mx-3 text-uppercase">
              <a :href="`${element.href}`">{{element.name}}</a>
          </li>
          <li>
              <a href="#" class="mx-3"><i class="fa-regular fa-user"></i></a>
          </li>
      </ul>
      <button type="button" class="btn text-uppercase button_color text-light fw-bold">get in touch</button>
  </div>
</template>

<script>
export default {
  //Cambiare il nome con quello del componente creato
  name: 'NavComp',
  data(){
      return {
          menuNav: [
              {
                  name: 'Home',
                  href: '#'
              },
              {
                  name: 'about',
                  href: '#'
              },
              {
                  name: 'services',
                  href: '#'
              },
              {
                  name: 'team',
                  href: '#'
              },
              {
                  name: 'blog',
                  href: '#'
              },
          ]
      }
  }

}
</script>

<style scoped lang="scss">
@import '../../style/variabili.scss';
 
 /*Inserire style componente*/
 ul{
     list-style: none;
     a{
         text-decoration: none;
         color: white;
     }
 }
 .button_color{
     background-color: $blue-lagoon;
 }
</style>