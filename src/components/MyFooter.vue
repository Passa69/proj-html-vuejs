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
}

</style>