<template>

<header class="text-center">
 <img  alt="Vue logo" src="../assets/images/la-molisana-logo.png">
 <nav class="container-fluid justify-content-between">
   <div class="row justify-content-center text-center">
   
    <div v-for="(items, index) in links" 
        :key="index" 
        :class="{'active' : items.active}" class="col-3 col-sm-2 col-lg-1 p-0 d-flex align-items-center justify-content-center"> 
        <span class="fw-bold p-2">{{items.testo}}</span>
        
    </div>
  
   </div>
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
span{
  font-size: 0.8em;
}
nav{
  color: white;
  background-color: $bg-navbar;
}

.active {
  color: black;
  background-color: $background;
}

</style>
