<template>
  <div class="card flex">
      <div class="date flex">
          {{CardDate[0]}}
          <div>{{CardDate[1]}},{{CardDate[2]}}</div>
      </div>
      <div class="flex text">
            <h3>{{CardTitle}}</h3>
            <div class="flex data-box">
                <div class="icon">ICN</div>    
                <div class="data">{{CardHours}}</div>
            </div>
            <div class="flex data-box">
                <div class="icon">ICN</div>    
                <div class="data">{{CardPlace}}</div>
            </div>
            <div>
                READ MORE
            </div>
      </div>
  </div>
</template>

<script>
export default {
    name:'EventCard',
    props: {
        CardDate: String,
        CardTitle: String,
        CardHours:String,
        CardPlace: String,
    }
}
</script>

<style lang="scss">
    .card{
        // background-color: rebeccapurple;
        padding:20px;
        border-bottom: solid #ececec ;
        border-width: 1px;
        .date{
            flex-basis: 25%;
            flex-direction: column;
            background-color: #ff4612;
            text-align: center;
            padding:5px;
            font-family: serif;
            font-size: 1.5rem;
            font-weight: 600;
            color:white;
            align-self: flex-start;
            div{
                font-size: 1rem;
                font-weight: 500;
            }
        }
        .text{
            width: 70%;
            flex-wrap: wrap;
            align-items: center;
            margin-left: 20px;
           
            h3{
                width: 100%;
                font-family: serif;
                font-size: 1.5rem;
            }
            .data-box{
                width: 100%;
                align-items: center;
                color: #8e8e8e;
                padding-top: 5px;
            }
            .icon{
                width: 10%;
                background-color: rosybrown;
            }
            .data{
                width: 90%;
                padding: 10px 0;
                padding-left: 8px;

            }
            >:last-child{
               padding-top:20px;
               font-weight: 600;
            }
        }
    }
</style>