<template>
  <section class="flex main-container">
      <div class="flex text-box">
          <h2>
              Creative Leader
          </h2>
          <div class="orange-underline"></div>
          <p>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Cumque, suscipit laboriosam sed facere at quibusdam, eligendi rem pariatur voluptates amet voluptas atque a illo eaque perferendis est porro excepturi inventore.
          </p>
          <strong>READ MORE</strong>
      </div>
      <div class="parameters">

      </div>
  </section>
</template>

<script>
export default {
    name: 'LeaderSection',

}
</script>

<style lang='scss' >
section{
    margin:auto;
    margin-top: 10vh;
}
.text-box{
    width: calc(90vw /2);
    flex-direction: column;
    h2{
        font-family: serif;
        font-size: 2rem;
        padding-bottom:10px ;
    }
    p{
        color: #8e8e8e;
        padding: 10px 0;
        line-height: 1.5rem;
        padding-right: 40px;
    }
    strong{
        padding-top: 10px;
        font-size: .85rem;
    }
}
.parameters{
    width: calc(90vw /2);
    height: 120px;
    background-color: rebeccapurple;
}
  
</style>