<template>
  <main>
    <!-- build team -->
    <section id="first">
      <div class="first_title">
        <h4>start learning coding lenguges</h4>

        <h1>Build Your Dream TODAY</h1>
      </div>

      <div class="card_container">
        <div v-for="(card, i) in cards" :key="i" class="card">
          <img :src="card.poster + '.png'" alt="">

          <h4><strong>{{ card.title }}</strong></h4>

          <p class="card_text">{{ card.text }}</p>
          <button class="card_button">Start now <i class="fas fa-long-arrow-alt-right"></i></button>
        </div>
      </div>
    </section>

    <!-- img+text -->

    <!-- statitics -->

    <!-- courses -->

    <!-- img+text -->

    <!-- img+text -->

    <!-- events -->

    <!-- love us -->
  </main>
</template>

<script>
export default {
  name: 'MyMain',
  data() {
    return {
      cards: [
        {
          poster: "@/assets/home-5-image-box-01",
          title: "Idea Discuss",
          text: "Lorem ipsum dolor sit amet consectetur adipisicing elit."
        },

        {
          poster: "@/assets/home-5-image-box-02",
          title: "Web Developer",
          text: "Lorem ipsum dolor sit amet consectetur adipisicing elit."
        },

        {
          poster: "@/assets/home-5-image-box-03",
          title: "System Administration",
          text: "Lorem ipsum dolor sit amet consectetur adipisicing elit."
        },

        {
          poster: "@/assets/home-5-image-box-04",
          title: "Graphic Design",
          text: "Lorem ipsum dolor sit amet consectetur adipisicing elit."
        },
      ]
    }
  }
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#first {
  margin: 50px 0;

  .first_title {
    margin-bottom: 50px;

    h4 {
      color: #8a8484;
      margin-bottom: 15px;
    }

    h1 {
      font-size: 40px;
    }
  }

  .card_container {
    display: flex;
    justify-content: space-around;

    .card {
      margin-right: 20px;

      h4 {
        color: #525252;
      }

      .card_text {
        margin: 20px 0;
        color: #b8b8b8;
      }

      .card_button {
        color: #9a98ad;
        background-color: white;
        border: none;
      }
    }
  }
}
</style>