<template>
<section class="flex our-specialties">
    <div class="flex main-container">
        <h2>
            Our specialties
        </h2>
        <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Totam minima beatae doloremque.
        </p>
        <span></span>
    </div>
    
</section>
 
</template>

<script>
export default {
    name: 'SpecialtiesSection'
}
</script>

<style lang="scss">
    .our-specialties {
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
</style>