<template>
  <div class="box">
      <ul>
          <li v-for="(element, index) in menuNav" :key="(index)">
              <a :href="`${element.href}`">{{element.name}}</a>
          </li>
          <li>
              <a href="#" class="mx-10"><i class="fa-regular fa-user"></i></a>
          </li>
      </ul>
      <button type="button" class="button_color button-all">get in touch</button>
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
//  utility
.mx-10{
  margin: 0 10px;
}
// fine utility
 .box{
     display: flex;
     justify-content: space-between;
     font-family: Arial, Helvetica, sans-serif;
 }
 ul{
     list-style: none;
     display: flex;
     align-items: center;
     li{
         text-transform: uppercase;
         margin: 0 10px;
     }
        a{
            text-decoration: none;
            color: white;
        }
 }
 .button_color{
     background-color: $blue-lagoon;
 }
 .button-all {
        text-transform: uppercase;
        color: #fff;
        padding: 10px 15px;
        border-radius: 5px;
        border: none;

    }
</style>