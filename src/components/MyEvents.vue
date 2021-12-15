<template>
    <section>
        <div style="width: 100%;">
          <h3 class="intest">Get in Contact Now</h3>

          <h1 id="title">Upcoming <span>Events</span></h1>

          <div id="events_cont">
              <div v-for="(event, i) in events" :key="i" id="event">
                  <div class="event_title">
                      <h4 class="intest"><i class="fas fa-map-marked-alt"></i> {{ event.place }}</h4>

                      <h2>{{ event.title }}</h2> 
                  </div>

                  <div class="date">
                      <h1 class="number">{{ event.day }}</h1>
                      <h3>{{ event.month }}</h3>

                      <button>Get Ticket</button>
                  </div>
              </div>
          </div>
          
          <h4 id="event_footer">Exited about our event? <a href="#">View all events <i class="fas fa-long-arrow-alt-right"></i></a></h4>
        </div>
    </section>
</template>

<script>
export default {
  name: 'MyEvents',
  data() {
      return {
          events:[
              {
                place: "Texas, US",
                title: "StoryTelling Workship",
                day: "22",
                month: "NOV", 
              },
              {
                place: "New York, US",
                title: "Painting Art Contest 2020",
                day: "10",
                month: "OCT", 
              },
              {
                place: "Hamburg, Germany",
                title: "International Art Fair 2020",
                day: "23",
                month: "OCT", 
              },
              {
                place: "Illinois, US",
                title: "Street Performance: Call for Artist",
                day: "15",
                month: "DEC", 
              },
              {
                place: "Illinois, US",
                title: "Consumer Food Safety Education Conference",
                day: "22",
                month: "JUL", 
              },
              {
                place: "Dubai",
                title: "How meditation improve your mental health?",
                day: "12",
                month: "AUG", 
              },
          ]
      }
  }
}
</script>

<style lang="scss">
.intest {
  color: #878a8b;
  margin-bottom: 10px;
}

#event_footer {
  color: #9a97ad;

  a {
    text-decoration: none;
    color: #2cb19b;
  }
}

#title {
  font-size: 40px;
  color: #3f3a64;

  span {
    color: #34ad96;
  }
}

#events_cont {
    display: flex;
    flex-flow: row wrap;
    justify-content: space-between;

    #event {
        display: flex;
        align-items: center;
        justify-content: space-between;
        width: 50%;
        margin: 30px 0;

        .event_title {
            text-align: left;
        }

        .date {
            .number {
                color: #34ad96;
            }

            button {
                padding: 15px;
                color: white;
                background-color: #20ad96;
                border: 1px solid #20ad96;
                border-radius: 10px;
                margin: 10px 0;
            }
        }

    }
}

</style>