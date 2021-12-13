<template>
  <nav>
      <!-- logo -->
      <img src="@/assets/dark-logo.png" alt="">

      <!-- links -->
      <ul>
          <li><a href="#">Home</a> <i class="fas fa-chevron-down"></i></li>
          <li><a href="#">Pages</a> <i class="fas fa-chevron-down"></i></li>
          <li><a href="#">Courses</a> <i class="fas fa-chevron-down"></i></li>
          <li><a href="#">Features</a> <i class="fas fa-chevron-down"></i></li>
          <li><a href="#">Blog</a> <i class="fas fa-chevron-down"></i></li>
          <li><a href="#">Shop</a> <i class="fas fa-chevron-down"></i></li>
      </ul>
  </nav>
</template>

<script>
export default {
  name: 'MyNavbar',
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
nav {
    // debug
    background-color: blue;
    height: 100px;
}
</style>