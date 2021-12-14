<template>
  <header>
    <!-- rendere dinamici props dall'app -->
    <!-- navbar -->
      <MyNavbar :links="navLinks"/>

    <!-- jumbotron -->
      <MyJumbo/>
  </header>
</template>

<script>
import MyNavbar from '@/components/MyNavbar.vue';
import MyJumbo from '@/components/MyJumbo.vue';


export default {
  name: 'MyHeader',
  components: {
    MyNavbar,
    MyJumbo
  },
  data() {
    return { 
      navLinks: ["Home", "Pages", "Courses", "Features", "Blog", "Shop"]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
header {
  width: 80%;
  margin: 0 auto;
}
</style>
