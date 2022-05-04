<template>

<footer>
    <h1>Sono il footer!</h1>
 </footer> 

</template>

<script>
export default {
  name: 'AppFooter',
  // props: {
  //   msg: String
  // }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
@import '../style/variables';
@import '../style/generals';


h1{
  background: $background;
  color: $fontColor;
  font-weight: 400;
}

</style>
