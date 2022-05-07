<template>
<div class="col-3">
    <img class="img-fluid" :src="item.src" alt="">
    <p class="fw-bold">{{item.titolo}}</p>
</div>
  
</template>

<script>
export default {
    name:'AppCard',
    props:{
       item: String 
    } 
}
</script>

<style lang="scss" scoped>
@import "../style/generals.scss";

.col-3{
    background-clip: border-box;
    
}
p{  padding: 0 10px;
    min-height: 50px;
    background-color: white;
    color: $bg-navbar;
}

</style>