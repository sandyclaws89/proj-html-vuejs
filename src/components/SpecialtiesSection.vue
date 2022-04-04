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
                    <span class="orange-underline"></span>
            </div>
        </div>
        <div class="flex methods-box">
            <div class="flex main-container">
                <ul class="flex">
                    <li v-for="(method, index) in arrMethods" :key="index" class="flex">
                        <div class="methods-text">
                            <!-- FIXME:SISTEMA CARICAMENTO IMG  -->
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
        <div class="flex interview-box">
            <div class="flex main-container">
                <div class="flex interview-slider">
                    <img src="../assets/img/h1-blog-img-04.jpg" alt="">

                    <div class="jason-profile">
                        <h2>
                            Jason Bickford
                        </h2>
                        <h3>Founder and Executive Director</h3>
                        <div class="orange-underline"></div>
                        <p>
                            Lorem ipsum dolor sit amet consectetur adipisicing elit. Esse, modi repudiandae recusandae et reiciendis odit aliquam earum laborum quas aliquid similique commodi
                        </p>
                        <div class="flex sign-social-box">
                            <div class="flex">
                                <span>
                                    IN
                                </span>
                                 <span>
                                    F
                                </span>
                                 <span>
                                    TW
                                </span>
                            </div>
                            <span>JASON BICKFORD SIGNED</span>
                        </div>
                    </div>
                    <img src="../assets/img/svg/svg-4.svg" alt="">
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
        padding-top: 150px;
        justify-content: center;
        // background-color: cadetblue;
        .interview-slider{
            justify-content: center;
            align-items: center;
            // padding-top: 200px;
            img{
                width:calc(90vw/2);
                height: 30rem;
            }
            .jason-profile{
                width: calc(90vw/2.5);
                height: 20rem;
                background-color: antiquewhite;
                padding: 50px 25px;
                margin-left: -100px;
                z-index: 555;
                h2{
                    font-family: serif;
                    font-size: 2rem;
                }
                h3{
                    font-size: 1rem;
                    padding: 10px 0;
                    font-weight: 200;
                }
                p{
                    padding: 15px 0;
                }
                .sign-social-box{
                    background-color: aqua;
                    width: 100%;
                    height: 25px;
                    justify-content: space-between;
                    span{
                        padding: 10px
                    }
                }
            }
            >:last-child{
                width: calc(90vw/3);
                margin-top: -200px;
                margin-left: -225px;
            }

        }
    }

    
    
</style>