<template>
  <div class="flex testimonial-card">
      <img :src="TestimonialImg" :alt="TestimonialName">
      <h4>{{TestimonialName}}</h4>
      <p>{{TestimonialText}}</p>
     
  </div>
</template>

<script>
export default {
    name: 'TestimonialsCard',
    props: {
        TestimonialName: String,
        TestimonialText: String,
        TestimonialImg: String
    }
}
</script>

<style lang="scss">
    .testimonial-card{
        flex-direction: column;
        color: white;
        align-items: center;
    }
</style>