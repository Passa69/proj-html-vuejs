<template>
  <nav>
      <!-- logo -->
      <img src="@/assets/dark-logo.png" alt="">

      <!-- links -->
      <ul v-for="(link, i) in links" :key="i">
          <li><a href="#">{{ link }}</a> <i class="fas fa-chevron-down"></i></li>

          <!-- <li><a href="#">Home</a> <i class="fas fa-chevron-down"></i></li>
          <li><a href="#">Pages</a> <i class="fas fa-chevron-down"></i></li>
          <li><a href="#">Courses</a> <i class="fas fa-chevron-down"></i></li>
          <li><a href="#">Features</a> <i class="fas fa-chevron-down"></i></li>
          <li><a href="#">Blog</a> <i class="fas fa-chevron-down"></i></li>
          <li><a href="#">Shop</a> <i class="fas fa-chevron-down"></i></li> -->
      </ul>

      <i class="far fa-user-circle"></i>

      <i class="fas fa-shopping-cart"></i>

      <input type="text" placeholder="Search...">
  </nav>
</template>

<script>
export default {
  name: 'MyNavbar',
  props: {
      links: Array
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
nav {
    display: flex;
    justify-content: space-around;
    align-items: center;
    height: 100px;

    img {
        height: 30px;
        width: 180px;
    }

    li {
        display: inline-block;
        margin: 10px;

        a {
            text-decoration: none;
            color: #605b7c;
            font-size: 18px;
        }
    }

    input {
        padding: 10px;
    }
}
</style>