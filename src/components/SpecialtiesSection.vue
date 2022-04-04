<template>
    <section>
        <div class="flex title-box">
            <div class="flex main-container">
                <h2>
                    Our specialties
                </h2>
                <p>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Totam minima      beatae doloremque.
                </p>
                    <span></span>
            </div>
        </div>
        <div class="flex methods-box">
            <div class="flex main-container">
                <ul class="flex">
                    <li v-for="(method, index) in arrMethods" :key="index" class="flex">
                        <div class="methods-text">
                            <!-- FIXME:SISTEMA CARIAMENTO IMG  -->
                            <img :src="method.img" :alt="title">
                            <h3>
                                {{method.title}}
                            </h3>
                            <span>{{method.text}}</span>
                        </div>
                    </li>
                </ul>
        </div>
        </div>
        <div class="flex interview box">
            <div class="flex main-container">
                <div class="interview-slider">
                     <img src="../assets/img/h1-blog-img-04.jpg" alt="">
                </div>
                
            </div>             
        </div>    
    </section>
    
</template>

<script>
export default {
    name: 'SpecialtiesSection',
    props: {
        
    },
    data() {
        return {
            arrMethods: [
                {         
                    title: 'Knowing',
                    text: 'lorem picsum lorem picsum lorem picsum lorem picsum',
                    img:  '../assets/img/h1-img-01.jpg',
                },
                {         
                    title: 'Selling',
                    text: 'lorem',
                    img:  '../assets/img/svg/svg-1.svg'
                },
                {         
                    title: 'Learning',
                    text: 'lorem picsum lorem picsum',
                    img:  '../assets/img/svg/svg-2.svg' 
                },
                {         
                    title: 'Contact',
                    text: 'lorem picsum',
                    img:  '../assets/img/svg/svg-3.svg' 
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    .title-box {
        justify-content: center;
        padding-top: 50px;
        align-items: center;
        // background-color: coral; 
        background-color: aquamarine;
        div{
            flex-direction: column;
            justify-content: center;
            align-items: center;
            width: 500px;
            background-color: cadetblue;
            h2{
                font-size: 2.5rem;
                padding-bottom: 10px;
            }
            p{
                padding-bottom: 25px;
            }
            span{
                width: 50px;
                border-radius: 40px;
                border: solid orangered;
                border-width: 2px;  
            }
        }
    }
    .methods-box {
        padding-top:50px ;
        justify-content: center;
        // width: 100%;
        ul{
            width: 100%;
            li{
                width: calc(90vw/4);
                justify-content: center;
                text-align: center;
                    .methods-text{
                        img{
                            display: block;
                            width: 150px;
                            height: 150px;
                        }
                       
                        h3{
                            display: inline;
                        }
                        span{
                            display: block;
                        }
                    }
            }
        }
    }
    .interview-box{
        margin-top: 200px;
        align-items: center;
        // justify-content: center;
        background-color: cadetblue;
        .interview-slider{
            justify-content: center;
            padding-top: 200px;
            img{
                width: 150px;
                height: 150px;
            }
        }
    }

    
    
</style>