<template>
  <section class="flex main-container news-card">
        <div class="flex img-news-box">
            <img :src="NewsImg" :alt="NewsTitle">
            <span>ICN</span>
            <span class="relative">{{NewsCategory}}</span>
        </div>
        <div class="flex data-news-box">
            <span>ICN</span>
            <span>{{NewsData}}</span>
            <span>ICN</span>
            <span>{{NewsAuthor}}</span>
        </div>
        <div class="flex content-news-box">
            <h3>
                {{NewsTitle}}
            </h3>
            <p>{{NewsContent}}</p>
            <strong>{{NewsOther}}</strong>
        </div>       
  </section>
</template>

<script>
export default {
    name: 'NewsCard',
    props: {
        NewsImg: String,
        NewsData: String,
        NewsAuthor: String,
        NewsTitle: String,
        NewsContent: String,
        NewsOther: String,
        NewsCategory: String
    }
}
</script>

<style lang="scss">
    .news-card{
        flex-direction: column;
        width: calc(90vw/3);
        align-items: flex-start;
        flex-wrap: wrap;
        margin-left: 10px;
        margin-right: 10px;
        .img-news-box{
            width: 100%;
            justify-content: end;
            flex-wrap: wrap;
            // background-color: brown;
            img{
                align-self: center;
                width: 100%;
                height: 200px;
                background-color: rosybrown;
            }
            span{
                display: inline-block;
                background-color: orangered;
                padding: 10px;
                margin-top: -20px;
                right: 10px;
                color: white;
                
            }
        }
        .data-news-box{
            span{
                padding: 5px;
            }
        }
        .content-news-box{
            width: 100%;
            background-color: aqua;
            flex-direction: column;
            height: 10rem;
            h3{
                font-family: serif;
                font-size: 1.5rem;
            }
            p{
                padding:10px 0;            
                width: 95%;
                overflow-wrap: break-word;
                flex-grow: 1;
                background-color: red;
            }
        }
    }
</style>