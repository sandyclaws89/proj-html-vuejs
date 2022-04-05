<template>
  <section class="flex">
      <div class="main-container flex">
          <div class="events-box relative">
              <h2>
                  Upcoming Events
              </h2>
              <EventCard
              v-for="(event, index) in arrEvents"
              :key="index"
              :CardDate="event.date"
              :CardTitle="event.event"
              :CardHours="event.hours"
              :CardPlace="event.place"
              />
          </div>
          <!-- <img src="../assets/img/h1-img-09.jpg" alt=""> -->
      </div>
  </section>
</template>

<script>
import EventCard from './EventCard.vue'
export default {
    name:'EventsSection',
    components: {
        EventCard
    },
    data() {
        return {
            arrEvents: [
                {
                    event:'Melbourne Coaching',
                    hours: '9:00 am - 5:00pm, jan 7, 2022',
                    place: 'Cambridge, MA 02138, USA',
                    date: ['07', 'jan','2022'],
                },
                 {
                    event:'New York Coaching',
                    hours: '9:00 am - 5:00pm, jan 7, 2022',
                    place: 'Cambridge, MA 02138, USA',
                    date: ['11', 'apr','2022'],
                },
                 {
                    event:'London Coaching',
                    hours: '9:00 am - 5:00pm, jan 7, 2022',
                    place: 'Cambridge, MA 02138, USA',
                    date: ['21', 'dec','2022'],
                },
                 {
                    event:'Berlin Coaching',
                    hours: '9:00 am - 5:00pm, jan 7, 2022',
                    place: 'Cambridge, MA 02138, USA',
                    date: ['18', 'jul','2022'],
                },
                 
                
                
                

            ],
        }
    }
}
</script>

<style lang='scss' scoped>
section{
        background-image: url('../assets/img/h1-img-09.jpg');
        background-size: cover;
        margin-top: 120px;
        width: calc(100vw - (100vw - 100%));
        height: 100vh; 
        justify-content: center;
        align-content: center;
        // position: relative;

        .main-container{
            align-items: center;
        }
         .events-box{
            width: 500px;
            height: 70%;
            background-color: white;
            overflow-y: scroll;
            overflow-x: hidden;
                h2{
                    width: 450px;
                    padding: 15px;
                    border-bottom: solid #efefef;
                    // TODO: NON RIESCO A DARE POSITION FIXED
                    // position: fixed;
                    // top: 0px;
                }
        }
}
   
</style>