<template>
  <footer>
    <!-- rendere dinamici props dall'app -->
    <section id="footer_up">
      <img src="@/assets/maxcoach-shape-01.png" alt="">

      <div>
        <h3 class="intest">Start today for getting <span>Online Certification</span></h3>

        <h1 class="up_title">You can be your own guiding star with our help!</h1>

        <button>Get started now</button>
      </div>

      <img src="@/assets/maxcoach-shape-02.png" alt="">
    </section>

    <section id="footer_down">
      <div>
        <ul v-for="(link, i) in links1" :key="i">
          <li><strong>{{ link.title }}</strong></li>
          <li><a href="#">{{ link.coordinates }}</a></li>
          <li><a href="#">{{ link.timetables }}</a></li>
          <li><a href="#">{{ link.mail }}</a></li>
        </ul>

        <!-- icon -->
        <div>
          <i class="fab fa-facebook-square"></i>
          <i class="fab fa-twitter"></i>
          <i class="fab fa-instagram"></i>
          <i class="fab fa-linkedin"></i>
        </div>
      </div>

      <div id="links">
        <ul v-for="(link, i) in links2" :key="i">
          <li><strong>{{ link.title }}</strong></li>
          <li><a href="#">{{ link.start }}</a></li>
          <li><a href="#">{{ link.blog }}</a></li>
          <li><a href="#">{{ link.info }}</a></li>
        </ul>

        <ul v-for="(link, i) in links3" :key="i" id="links_no">
          <li><a href="#">{{ link.story }}</a></li>
          <li><a href="#">{{ link.culture }}</a></li>
          <li><a href="#">{{ link.contact }}</a></li>
        </ul>

        <ul v-for="(link, i) in links4" :key="i">
          <li><strong>{{ link.title }}</strong></li>
          <li><a href="#">{{ link.member }}</a></li>
          <li><a href="#">{{ link.guide }}</a></li>
          <li><a href="#">{{ link.police }}</a></li>
          <li><a href="#">{{ link.service }}</a></li>
        </ul>
      </div>
    </section>

    <h5>2020 Maxcoach. All Rights Reserved</h5>
  </footer>
</template>

<script>
export default {
  name: 'MyFooter',
  props: {
    links1: Array,
    links2: Array,
    links3: Array,
    links4: Array
  }
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
footer {
  padding: 50px 0;

  #footer_up {
    display: flex;
    justify-content: space-around;
    align-items: center;
    margin-bottom: 100px;
    color: #3f3a64;

    .up_title {
      font-size: 30px;
      margin: 10px;
    }

    span {
      color: #51bdab;
    }

    button {
      margin-top: 30px;
      padding: 15px 70px;
      color: white;
      background-color: #20ad96;
      border: 1px solid #20ad96;
      border-radius: 5px;
    }
  }

  #footer_down {
    display: flex;
    justify-content: space-around;
    padding: 50px 0;
    text-align: left;

    #links {
      display: flex;
      justify-content: space-around;

      #links_no {
        margin-top: 40px;
      }
    }

    ul {
      list-style-type: none;

      li {
        margin: 20px;

        a {
          text-decoration: none;
          color: #7e7e7e;
        }
      }
    }

    i {
      font-size: 30px;
      margin: 20px;
      color: #b4b4b4;
    }
  }

  h5 {
    color: #b7b7b7;
  }
}

</style>