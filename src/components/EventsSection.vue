<template>
  <section class="flex">
      <div class="main-container flex">
          <div class="events-box">

          </div>
          <!-- <img src="../assets/img/h1-img-09.jpg" alt=""> -->
      </div>
  </section>
</template>

<script>
export default {
    name:'EventsSection',
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
             background-color: chocolate;
            //  padding-left: 25px;
           
        }
}
   
</style>