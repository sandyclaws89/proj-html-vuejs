<template>
  <div class="flex relative testimonial-card">
      <div class="flex box-testimonial-img">
          <img :src="TestimonialImg" :alt="TestimonialName">
      </div>
      
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
        // justify-content: flex-start;
        // background-color: red;
        bottom: 100px;
        .box-testimonial-img{
            width: 100px;
            height: 100px;
            background-color: yellowgreen;
            border-radius: 50%;
            background-position: center;
            align-items: center;
            justify-content: center;
        }
        h4{
            font-family: serif;
            padding: 10px 0;
        }
        
    }
</style>