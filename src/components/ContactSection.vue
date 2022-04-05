<template>
  <section class="flex main-container">
      <div class="flex map">
          <img src="../assets/img/h1-contact-rev-01.png" alt="">
      </div>
      <div class="flex contact-us">
            <h2>
              Contact Us
            </h2>
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit.</p>
            <div class="orange-underline"></div>
            <div class="flex input-box">
              <input type="text" placeholder="Your Name">
              <input type="email" placeholder="Your Email">
              <input type="text" placeholder="Write a message...">
            </div>
            <button class="flex">
                Send
                <div></div>
                <span>ICN</span>
            </button>
      </div>
  </section>
</template>

<script>
export default {
    name: 'ContactSection'
}
</script>

<style lang ="scss" scoped>
    section{
        justify-content: center;
        align-items: center;
        /* margin: 0 20px; */
       
        .map{
            width: 50%;
            /* background-color: red; */
            justify-content: center;
            /* margin-right: 20px; */
        }
        .contact-us{
            flex-direction: column;
            width: 50%;
             /* margin-left: 20px; */
            /* background-color: aquamarine; */
            h2 {
                font-family: serif;
            }
            p {
                color: #8e8e8e;
                padding:10px 0;
            }  
            .input-box{
                flex-wrap: wrap;
                input{
                    width: calc(50% - 20px);
                    border: 0px;
                    border-bottom:solid #cccccc;
                    border-width: 1.5px;
                    padding: 5px;
                    margin: 10px;
                }
                :last-child{
                    flex-grow: 1;
                    line-height: 100px;
                   
                    vertical-align: text-bottom;
                }
                :last-child::placeholder{
                    position: relative;
                    bottom: 40px;
                }
            }
            button{
                width: 200px;
                height: 50px;
                align-items: center;
                justify-content: space-around;
                padding: 15px;
                background-color: orangered;
                border: none;
                color: white;
                div{
                    height: 40px;
                    width: 1px;
                    background-color: white;
                }
            }
        }
    }
    
                    



</style>