<template>
  <section>
    <div>
        <h3>Choose where you'd like to begin</h3>

        <h1>Latest Feautered <span>Courses</span></h1>

        <div id="corses_cont" style="width: 100%; margin: 50px 0;">
          <div v-for="(course, i) in courses" :key="i" id="courses">
            <img :src="require('@/assets/' + course.path)" alt="">

            <span class="price">{{ course.price }}</span>

            <div>
                <!-- <div>
                    <img :src="require('@/assets/' + course.profile)" alt="">
                </div> -->

                <span>{{ course.name }}</span>

                <h4><strong>{{ course.title }}</strong></h4>

                <span class="freq"><i class="far fa-file-alt"></i> {{ course.lesson }}</span>
                <span class="freq"><i class="far fa-user"></i> {{ course.student }}</span>
            </div>
          </div>
        </div>
        
    </div>
  </section>
</template>

<script>
export default {
  name: 'MyCourses',
  data() {
      return {
          courses: [
              {
                path: "course-02-480x298.jpg",
                price: "$40.00",
                profile: "",
                name: "Blanche Fields",
                title: "Learning to write as a Professional Author",
                lesson: "20 Lessons",
                student: "50 Students"
              },
              {
                path: "stock-full-hd-03-480x298.jpg",
                price: "Free",
                profile: "",
                name: "Maggie Strickland",
                title: "Costumer-centric info-Tech Strategies",
                lesson: "24 Lessons",
                student: "769 Students"
              },
              {
                path: "stock-full-hd-04-480x298.jpg",
                price: "$19.00",
                profile: "",
                name: "Maggie Strickland",
                title: "Open Programming Courses for Everyone",
                lesson: "17 Lessons",
                student: "62 Students"
              },
              {
                path: "stock-full-hd-06-480x298.jpg",
                price: "$26.00",
                profile: "",
                name: "Blanche Fields",
                title: "Academic Listening and Note-taking",
                lesson: "14 Lessons",
                student: "67 Students"
              },
              {
                path: "course-featured-image-01-480x298.jpg",
                price: "$39.00",
                profile: "",
                name: "Blanche Fields",
                title: "Master jQuery in a Shot Period of Time",
                lesson: "6 Lessons",
                student: "51 Students"
              },
              {
                path: "stock-full-hd-05-480x298.jpg",
                price: "$59.00",
                profile: "",
                name: "Blanche Fields",
                title: "Introduction to Javascript for Beginners",
                lesson: "14 Lessons",
                student: "76 Students"
              },
          ]
      }
  }

}
</script>

<style lang="scss">
h3 {
  color: #878a8b;
  margin-bottom: 10px;
}

h1 {
  font-size: 40px;
  color: #3f3a64;

  span {
    color: #34ad96;
  }
}

#corses_cont {
    display: flex;
    flex-flow: row wrap;
    justify-content: space-around;

    #courses {
      width: 30%;
      margin-bottom: 20px;

      img {
        width: 100%;
      }
      
      h4 {
        margin: 15px 0;
      }

      .freq {
        margin-right: 10px;
        color: #8b8b8b;
      }
    }

    div {
      position: relative;
      
      .price {
        padding: 10px;
        color: white;
        background-color: #20ad96;
        position: absolute;
        top: 0;
        right: 0;
      } 
    }
}
</style>
