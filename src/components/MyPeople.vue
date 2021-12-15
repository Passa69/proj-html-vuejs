<template>
  <section id="people">
        <h3 class="intest">People are praising Maxcoach</h3>

        <h1>What make they <span>Love Us?</span></h1>

        <div class="people_cont">
            <div v-for="(people, i) in peoples" :key="i">
                <div class="cont">
                    <div class="people_img">
                        <img :src="require('@/assets/' + people.picture)" alt="">
                    </div>

                    <p>{{ people.text }}</p>

                    <h4>{{ people.name }}</h4>

                    <span>{{ people.work }}</span>
                </div>
            </div>
        </div>

        <i class="fas fa-ellipsis-h" style="font-size: 45px;"></i>
  </section>
</template>

<script>
export default {
  name: 'MyPeople',
  data() {
      return {
          peoples: [
              {
                picture: "testimonial-avata-02.jpg",
                text: "Iure doloremque voluptate ipsa architecto, provident facere harum quisquam ab consectetur eveniet veniam nostrum cupiditate fugiat velit ad temporibus corrupti, placeat ex.",
                name: "MINA HOLLACE",
                work: "/ Freelancer"
              },
              {
                picture: "testimonial-avata-04.jpg",
                text: "Lorem ipsum dolor sit amet consectetur, adipisicing elit. Iure doloremque voluptate ipsa architecto, provident facere harum quisquam ab consectetur eveniet veniam nostrum cupiditate fugiat velit ad temporibus corrupti, placeat ex.",
                name: "MADLEY PONDOR",
                work: "/ IT Specialist"
              },
              {
                picture: "testimonial-avata-01.jpg",
                text: "Lorem ipsum dolor sit amet consectetur, adipisicing elit. Iure doloremque voluptate ipsa architecto.",
                name: "LUVIC DUBBLE",
                work: "/ Private Tutor"
              },
          ]
      }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#people {
    margin: 40px 0;

    .people_cont {
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        width: 100%;
        margin: 50px 0;

        .people_img {
            width: 150px;

            img {
                border-radius: 50%;
                margin: 15px 0;
                width: 100%;
                height: 100%;
            }
        }

        p {
            color: #676384;
            margin: 15px 0;
        }

        h4 {
            margin: 10px 0;
        }

        span {
            color: #ababab;
            font-size: 15px;
        }
    }
}
</style>