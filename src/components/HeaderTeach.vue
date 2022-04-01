<template>
<!--TODO:FARE LO SLIDE -->
<header class="flex">
    <nav class="flex main-container">
        <img src="../assets/img/logo-img-01.png" alt="">
        <ul>
            <li v-for="(category, index) in arrHeaderNav" :key="index">{{category.categories}}</li>
            <li>ICN</li> <!--TODO:CERCA SVG -->
            <li>ICN</li> <!--TODO:CERCA SVG -->
        </ul>
    </nav>
    <section class="main-container flex jumbotron">
        <!--TODO:SISTEMA BENE STILE -->
        <span>ICONS</span>
        <div>
            <h1>
                Our team
            </h1>
            <p>
                Lorem, ipsum dolor sit amet consectetur adipisicing elit. Est rerum quo nam aspernatur sit itaque odit soluta hic.
            </p>
            <button>READ MORE</button>
            <button>PURCHASE</button>
        </div>
       
        <span>ICONS</span>
    </section>
</header>
</template>

<script>
export default {
    name:'HeaderTeach',
    data() {
        return {
            arrHeaderNav: [
                {
                    categories: 'HOMES',
                    subcatergories1: 'textsub1',
                    subcatergories2: 'textsub2',
                    subcatergories3: 'textsub3',
                },
                {
                    categories: 'PAGES',
                    subcatergories1: 'textsub1',
                    subcatergories2: 'textsub2',
                    subcatergories3: 'textsub3',
                },
                {
                    categories: 'BLOG',
                    subcatergories1: 'textsub1',
                    subcatergories2: 'textsub2',
                    subcatergories3: 'textsub3',
                },
                {
                    categories: 'SHOP',
                    subcatergories1: 'textsub1',
                    subcatergories2: 'textsub2',
                    subcatergories3: 'textsub3',
                },
                {
                    categories: 'EVENTS',
                    subcatergories1: 'textsub1',
                    subcatergories2: 'textsub2',
                    subcatergories3: 'textsub3',
                },
                {
                    categories: 'ELEMENTS',
                    subcatergories1: 'textsub1',
                    subcatergories2: 'textsub2',
                    subcatergories3: 'textsub3',
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
header{
    background-image: url('../assets/img/rev-slider-main-home-img-03.jpg');
    justify-content: center;
    height: 90vh;
    background-position: center;
    flex-wrap: wrap;
    nav{
        height: 50px;
        justify-content: space-between;
        align-items: center;
        img{
            height: 50%;
        }
        li{
            display: inline; 
            padding: 0 15px;
            font-weight: 500;
        }
    }

    .jumbotron{
        justify-content: space-between;
        align-items: flex-start;
        div{
            margin-left: -500px;
            width: 400px;
            h1{
            font-size: 4rem;
            font-family: serif;
            width: 70%;
            }
            p{
             padding-top: 10px;
             width: 50%;
            }
            button{
                width: 50%;
                height: 30px;
            }
        }  
    }
    

}
</style>