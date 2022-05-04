<template>

<header>
 <img alt="Vue logo" src="../assets/images/la-molisana-logo.png">
 <nav>
   <ul>
     <li  
        v-for="(items, index) in links" 
        :key="index" 
        :class="{'active' : items.active}"> {{items.testo}}
     </li>
   </ul>
 </nav>
 </header> 
 
</template>

<script>
export default {
  name: 'AppHeader',
  data(){
    return{
      links:[
        {
          testo:"Home",
          link:"",
          active: false
        },
        {
          testo:"Prodotti",
          link:"",
          active: true
        },
        {
          testo:"Chi Siamo",
          link:"",
          active: false
        },
        {
          testo:"Contatti",
          link:"",
          active: false
        }
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
@import '../style/variables';
@import '../style/generals';


.active {
  background-color: $background;
}

</style>
