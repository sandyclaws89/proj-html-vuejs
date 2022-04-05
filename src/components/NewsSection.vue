<template>
  <section class="main-container">
        <img src="../assets/img/svg/svg-4.svg" alt="" class="relative">
        <div class="flex title-news">
            <h2> Latest news </h2>
            <p> Lorem ipsum, dolor sit amet consectetur adipisicing elit.</p>
            <div class="orange-underline"></div>
        </div>
        <div class="flex slide-news">
            <NewsCard
            v-for="(news, index) in arrNews"
            :key="index"
            :news-img = news.img
            :news-data = news.data
            :news-author = news.author
            :news-title = news.name
            :news-content = news.content
            :news-other = news.other
            />
        </div>
      
  </section>
</template>

<script>
import NewsCard from './NewsCard.vue'
export default {
    name: 'NewsSection',
     components: {
        NewsCard
    },
    data() {
        return {
            arrNews:[
                {
                    name:'Next investment',
                    content:'aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa',
                    img: '../assets/img/h1-blog-img-02.jpg',
                    data: 'May 5, 2019',
                    author: 'Amanda Doe',
                    category: 'Business Leading', 
                    other: 'READ MORE'
                },
                {
                    name:'Team Building',
                    content:'bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb',
                    img: '../assets/img/h1-blog-img-03.jpg',
                    data: 'Gen 15, 2018',
                    author: 'John Black',
                    category: 'Business Leading', 
                    other: 'READ MORE'
                },
                 {
                    name:'New Business Day',
                    content:'ccccccccccccccccccccccccccc',
                    img: '../assets/img/h1-blog-img-01.jpg',
                    data: 'ago 31, 2021',
                    author: 'Frederic Terry',
                    category: 'Business Leading', 
                    other: 'READ MORE'
                },
            ]
        }
    }

}
</script>

<style lang="scss" scoped>
    section{
        img{
            left: 70px;
        }
        .title-news{
            margin-top: -150px;
            flex-direction: column;
            align-items: center;
            // background-color: blue;
           
            h2{
                font-family: serif;
                font-size: 2rem;
            }
            p{
                padding:15px 0;
                color: #8e8e8e;
            }
        }
        .slide-news{
            // background-color: red;
        }
    }
</style>