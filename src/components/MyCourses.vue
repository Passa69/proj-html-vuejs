<template>
  <section id="corses_cont">
    <div>
        <h3>Choose where you'd like to begin</h3>

        <h1>Latest Feautered <span>Courses</span></h1>

        <div>
            <img src="@/assets/course-02-480x298.jpg" alt="">

            <span class="price">$40.00</span>

            <div>
                <div>
                    <img src="" alt="">
                </div>

                <span>Blanche Fields</span>

                <h4><strong>Learning to write as a Professional Author</strong></h4>

                <span><i class="far fa-file-alt"></i> 20 Lessons</span>
                <span><i class="far fa-user"></i> 50 Students</span>
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
                path: "@/assets/course-02-480x298.jpg",
                profile: "",
                name: "Blanche Fields",
                title: "Learning to write as a Professional Author",
                lesson: "20 Lessons",
                student: "50 Students"
              },
              {
                path: "",
                profile: "",
                name: "",
                title: "",
                lesson: "",
                student: ""
              },
              {
                path: "",
                profile: "",
                name: "",
                title: "",
                lesson: "",
                student: ""
              },
              {
                path: "",
                profile: "",
                name: "",
                title: "",
                lesson: "",
                student: ""
              },
              {
                path: "",
                profile: "",
                name: "",
                title: "",
                lesson: "",
                student: ""
              },
              {
                path: "",
                profile: "",
                name: "",
                title: "",
                lesson: "",
                student: ""
              },
          ]
      }
  }

}
</script>

<style lang="scss">
#corses_cont {
    margin: 50px 0;
    display: flex;
    flex-flow: row wrap;
    justify-content: space-between;

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
}

div {
        position: relative;   
}

.price {
    padding: 10px;
    color: white;
    background-color: #20ad96;
    position: absolute;
    top: 0;
    right: 0;
}
</style>
