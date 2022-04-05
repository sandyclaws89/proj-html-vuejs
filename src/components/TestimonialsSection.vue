<template>
  <section class="banner flex">
    <span>Testimonials</span>
      <TestimonialsCard
        v-for="(testimonial, index) in arrTestimonials"
        :key="index"
        :testimonial-name = testimonial.name
        :testimonial-text = testimonial.testimonial
        :testimonial-img = testimonial.img  
      />
  </section>
</template>

<script>
import TestimonialsCard from './TestimonialsCard.vue'
export default {
    name: 'TestimonialsSection',
    components: {
        TestimonialsCard
    },
    data() {
      return {
        arrTestimonials: [
          {
            name: 'Cynthia Clark',
            testimonial: 'lorem ipsum dolor sit amet, consectetur adipiscing elit sed eiusmod tempor incididunt ut labore et dolore magna aliqua',
            img: '../assets/img/h3-img-04.png'
          },
          {
            name: 'Cindy Sullivan',
            testimonial: 'lorem ipsum dolor sit amet',
            img: '../assets/img/h3-img-07.png'
          },
          {
            name: 'Lisey Landon',
            testimonial: 'lorem ipsum dolor sit amet lorem ipsum dolor sit amet, consectetur adipiscing elit sed eiusmod tempor incididunt ut labore et dolore magna aliqua',
            img: '../assets/img/h3-img-08.png'
          },
        ]
      }
    },
}
</script>

<style lang="scss">
  .banner{
    margin-top: 100px;
    background-color: #1e1c1c;
    height: 50vh;
    width: 100%;
    justify-content: center;
    align-items: flex-start;
    flex-wrap: wrap;
    span{
      font-size: 15rem;
      font-family: serif;
      line-height: 12rem;
    }
    
  }
</style>