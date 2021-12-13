<template>
  <header>
    <!-- navbar -->
      <MyNavbar/>

    <!-- jumbotron -->
      <!-- text -->

      <!-- immagine -->
  </header>
</template>

<script>
import MyNavbar from '@/components/MyNavbar.vue';


export default {
  name: 'MyHeader',
  components: {
    MyNavbar,
  } 
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
header {
  // debug
  background-color: red;
  height: 500px;
}
</style>
