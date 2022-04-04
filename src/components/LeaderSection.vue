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
      <div class="parameters flex">
          <div v-for="(element, index) in arrParameters" :key="index" class="parameter-card">
              <div class="flex">
                    <h3>{{element.parameter}}</h3>
                    <strong>{{`${element.value}%`}}</strong>
              </div>
              <div class="bar">
                  <!-- <div :style="width{{element}}"></div> -->
              </div>
          </div>
      </div>
  </section>
</template>

<script>
export default {
    name: 'LeaderSection',
    data() {
        return{
            arrParameters: [
            {
                parameter: 'Mentorship',
                value: 78,
            },
            {
                parameter: 'Education',
                value: 95,
            },
            {
                parameter: 'Learning',
                value: 65,
            },
            {
                parameter: 'Motivation',
                value: 83,
            },

            ] 
        }
    }
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
    flex-direction: column;
    width: calc(90vw /2);
    height: 120px;
    background-color: rebeccapurple;
   
    .parameter-card{
        padding: 10px 0;
        >:first-child{
            justify-content: space-between;
            font-family: serif;
            h3{
                font-family: serif;
            }
            strong{
                font-family: serif;
            }
        }
        .bar{
            margin-top: 5px;
            width:calc(90vw /2);
            background-color: #e1e1e1;
            height: 2px;
            justify-content: space-between;

            div{
                width: 78%;
                background-color: orangered;
                height: 2px;
            }
        }
    }
}
  
</style>