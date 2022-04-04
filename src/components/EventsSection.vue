<template>
  <section class="flex">
      <div class="main-container flex">
          <div class="events-box">
              <h2>
                  Upcoming Events
              </h2>
              <EventCard/>
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
        .main-container{
            align-items: center;
        }
         .events-box{
            width: 300px;
            height: 60%;
            background-color: white;
                h2{
                    padding: 15px;
                    border-bottom: solid #efefef;
                }
        }
}
   
</style>