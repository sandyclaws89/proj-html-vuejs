<template>
<header class="flex">
    <nav class="flex main-container">

    </nav>
</header>
</template>

<script>
export default {
    name:'HeaderTeach',
    data() {
        return {
            arrHeaderNav: [
                {
                    categories: 'homes',
                    subcatergories1: 'textsub1',
                    subcatergories2: 'textsub2',
                    subcatergories3: 'textsub3',
                },
                {
                    categories: 'pages',
                    subcatergories1: 'textsub1',
                    subcatergories2: 'textsub2',
                    subcatergories3: 'textsub3',
                },
                {
                    categories: 'blog',
                    subcatergories1: 'textsub1',
                    subcatergories2: 'textsub2',
                    subcatergories3: 'textsub3',
                },
                {
                    categories: 'shop',
                    subcatergories1: 'textsub1',
                    subcatergories2: 'textsub2',
                    subcatergories3: 'textsub3',
                },
                {
                    categories: 'events',
                    subcatergories1: 'textsub1',
                    subcatergories2: 'textsub2',
                    subcatergories3: 'textsub3',
                },
                {
                    categories: 'elements',
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
    width: 100%;
    height: 90vh;
    background-position: center;
    nav{
        height: 50px;
        background-color: rebeccapurple;
        justify-content: center;
    }
    .jumbotron{
        
        
        justify-content: center;
       
        object-fit:fill
    }

}
</style>