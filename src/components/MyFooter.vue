<template>
  <footer>
    <section id="footer_up">
      <img src="@/assets/maxcoach-shape-01.png" alt="">

      <div>
        <h3>Start today for getting <span>Online Certification</span></h3>

        <h1 class="up_title">You can be your own guiding star with our help!</h1>

        <button>Get started now</button>
      </div>

      <img src="@/assets/maxcoach-shape-02.png" alt="">
    </section>

    <section id="footer_down">
      <div>
        <ul>
          <li><strong>Address</strong></li>
          <li><a href="#">382 NE 191st St # 87394 Miami, FL 33179-3899</a></li>
          <li><a href="#">+1 (305) 547-9909 (9am-5pm EST, Monday-Friday)</a></li>
          <li><a href="#">support@maxcoach.com</a></li>
        </ul>

        <!-- icon -->
        <div></div>
      </div>

      <div id="links">
        <ul>
          <li><strong>Explore</strong></li>
          <li><a href="#">Start here</a></li>
          <li><a href="#">Blog</a></li>
          <li><a href="#">About us</a></li>
        </ul>

        <ul id="links_no">
          <li><a href="#">Success story</a></li>
          <li><a href="#">Courses</a></li>
          <li><a href="#">Contact us</a></li>
        </ul>

        <ul>
          <li><strong>Information</strong></li>
          <li><a href="#">Membership</a></li>
          <li><a href="#">Purchase guide</a></li>
          <li><a href="#">Privacy police</a></li>
          <li><a href="#">Terms of service</a></li>
        </ul>
      </div>
    </section>

    <h5>2020 Maxcoach. All Rights Reserved</h5>
  </footer>
</template>

<script>
export default {
  name: 'MyFooter',
  
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
  }

  h5 {
    color: #b7b7b7;
  }
}

</style>