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
          <img :src="require('../assets/'+card.poster)" alt="">

          <h4><strong>{{ card.title }}</strong></h4>

          <p class="card_text">{{ card.text }}</p>
          <button class="card_button">Start now <i class="fas fa-long-arrow-alt-right"></i></button>
        </div>
      </div>
    </section>

    <!-- img+text -->
    <section class="container_info">
      <img src="@/assets/about-us-03-image-01.png" alt="">

      <div class="info_text">
        <h3 class="dream">Dream with <strong>MAXCOACH</strong></h3>

        <h1 class="info_title">Construct A <span>Stunning</span> Career Perspective</h1>

        <h4 class="selected">Multiple Platforms Supported for Teaching and Studing <i class="fas fa-minus-circle"></i></h4>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. At natus in voluptate dolor quibusdam qui ab, dolorum, eum quam quae velit vero quia ratione, nostrum est? Velit maxime commodi pariatur.</p>

        <h4>Multiple Course Partecipation at the Same Time <i class="fas fa-plus-circle"></i></h4>

        <h4>Track Study Progress and Deliver Prompt Feedback <i class="fas fa-plus-circle"></i></h4>
      </div>
    </section>

    <!-- statitics -->
    <section class="stat_container">
      <div v-for="(stat, i) in stats" :key="i">
        <h1>{{ stat.numb }}</h1>
        <h2>{{ stat.name }}</h2>
      </div>
    </section>

    <!-- courses -->
    <MyCourses/>

    <!-- img+text -->
    <section class="container_info">
      <div class="info_text">
        <h3 class="dream">Why esitate for register?</h3>

        <h1 class="info_title">Learn at your Own <span>Place</span></h1>

        <ul>
          <li><i class="fas fa-check"></i> Select and costumize courses to your preferences</li>
          <li><i class="fas fa-check"></i> Cahnge te tutor and make arrangements</li>
          <li><i class="fas fa-check"></i> Partecipate in events to join others</li>
          <li><i class="fas fa-check"></i> Get the disired certificate delivered at house</li>
        </ul>

        <button>Get started for free</button>
      </div>

      <img src="@/assets/home-5-image-01.png" alt="">
    </section>

    <!-- img+text -->
    <section class="container_info">
      <img src="@/assets/home-5-image-02.png" alt="">

      <div class="info_text">
        <h3 class="dream">What are you looking for?</h3>

        <h1 class="info_title">Learn on your <span>Mobile</span> Anytime!</h1>

        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Iure ab vitae quas odit eius, labore, consequatur obcaecati harum ut corrupti deserunt necessitatibus perferendis debitis nostrum nisi unde cumque. Laboriosam, officia. Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quod, nihil. Et nemo unde nulla reiciendis tenetur a eveniet ipsam pariatur eum illum voluptatum iste accusamus error, quidem repellat dolore libero.</p>

        <button>Download our app</button>
      </div>
    </section>

    <!-- events -->
    

    <!-- love us -->
    
  </main>
</template>

<script>
import MyCourses from '@/components/MyCourses.vue';

export default {
  name: 'MyMain',
  components: {
    MyCourses
  },
  data() {
    return {
      cards: [
        {
          poster: "home-5-image-box-01.png",
          title: "Idea Discuss",
          text: "Lorem ipsum dolor sit amet consectetur adipisicing elit."
        },

        {
          poster: "home-5-image-box-02.png",
          title: "Web Developer",
          text: "Lorem ipsum dolor sit amet consectetur adipisicing elit."
        },

        {
          poster: "home-5-image-box-03.png",
          title: "System Administration",
          text: "Lorem ipsum dolor sit amet consectetur adipisicing elit."
        },

        {
          poster: "home-5-image-box-04.png",
          title: "Graphic Design",
          text: "Lorem ipsum dolor sit amet consectetur adipisicing elit."
        },
      ],
      stats: [
        {
          numb: "1.926",
          name: "Finished Lesson"
        },
        {
          numb: "3.092+",
          name: "Enrolled Learners"
        },
        {
          numb: "200",
          name: "Online Instructors"
        },
        {
          numb: "100%",
          name: "Satisfation Rate"
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

.container_info {
  display: flex;
  justify-content: space-between;

  div {
    padding: 50px;
  }

  .info_text {
    display: flex;
    flex-direction: column;
    justify-content: center;
    text-align: left;

    h4, p {
      padding: 20px;
      position: relative;
    }

    .fa-plus-circle, .fa-minus-circle {
      position: absolute;
      top: 35%;
      right: 10px;
    }

    ul {
      list-style-type: none;
      padding: 20px;

      li {
        padding: 10px 0;
        
        i {
          color: #27af99;
        }
      }
    }

    .selected {
      color: white;
      background-color: #62c5b5;
    }

    button {
      padding: 15px 20px;
      color: white;
      background-color: #20ad96;
      border: 1px solid #20ad96;
      border-radius: 10px;
      margin: 10px 20px;
      width: 200px;
    }
  }
  
}

.dream {
  color: #6e6a6b;
  margin-bottom: 10px;
}

.info_title {
  font-size: 40px;
  color: #545275;
  margin-bottom: 30px;

  span {
    color: #42bebe;
  }
}

.stat_container {
  display: flex;
  justify-content: space-around;
  margin: 50px 0;

  h1 {
    font-size: 30px;
    color: #27ad96;
  }

  h2 {
    font-size: 15px;
    color: #555a78;
  }
}
</style>