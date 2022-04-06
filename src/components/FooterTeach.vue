<template>
  <section class="flex">   
    <ul class="main-container flex">
      <li  class="list-title">
        <h3>
          About
        </h3>
        <div class="orange-underline"></div>
        <p>
          We created Everlead to effectively become the stepping stone towards meeting all your goals & achieving business success.
        </p>
        <div class=" flex social-logo-box">
          <div>IN</div>
          <div>F</div>
          <div>TW</div>
        </div>
      </li>
      <li class="list-title">
        <h3>
          Twitter
        </h3>
        <div class="orange-underline"></div>
        <div v-for="(tweet, index) in arrTweet"
        :key="index" class="twitter-list">
          <p>
            {{`@${tweet.user}`}} {{tweet.tweet}}
          </p>
        </div>
      </li>
      <li class="list-title ">
        <h3>
          Important links
        </h3>
        <div class="orange-underline"></div>
        <ul>
          <li v-for="(link, index) in arrLinks"
          :key="index" class="link-list">
            {{link}}
          </li>
        </ul>
      </li>
      <li class="list-title">
        <h3>
          Contact me
        </h3>
        <div class="orange-underline"></div>
        <ul>
          <li v-for="(contact,index) in arrContact"
          :key="index" class="contact-list">
            <span>{{contact.icon}} {{contact.text}}</span>
          </li>
        </ul>
      </li>
    </ul>
  </section>
</template>

<script>
export default {
    name: 'FooterTeach',
    data() {
      return {
        arrTitle: ['About', 'Twitter', 'Important links', 'Contact me'],
        arrTweet: [
          {
            user:'aliasdadm',
            tweet: 'Hi @aliasdadm, can you please submit a ticket at https://t.co/JLV61aXG7d and one of our support agent... https://t.co/yk57k1S9bS'
          },
          {
            user:'HenrySefaBoaky1',
            tweet: 'Check out our theme Gioia which has all necessary elements to build a multi vendor marketplace. https://t.co/c)BlYxZBlL'
          },
        ],
        arrLinks: ['About me','About us', 'Language packs','Become a coach', 'Monthly events'],
        arrContact: [
          {
            icon: 'ICN',
            type: 'place',
            text: '457 BigBlue Street, NY 10013',
          },
          {
            icon: 'ICN',
            type: 'tel',
            text: '(315)5512-2579',
          },
          {
            icon: 'ICN',
            type: 'email',
            text: 'everlad@mikado.com',
          },

        ]
      }
    }
}
</script>

<style lang ="scss" scoped>
section{
  justify-content: center;
  height: 50vh;
  background-color: black;
  align-items: flex-start;
  color: #8e8e8e;
  ul{
    padding:20px 0 ;
  }
  p{
    padding: 10px 0;
  }

  .list-title{
    width: calc(100% / 4);
    display: inline-block;
    background-color: darkblue;
    padding:15px;

    h3{
      font-family: serif;
      color: white;
    }
    .link-list{
       list-style: none;
        /* padding: 10px 0; */
    }
    .contact-list{
       list-style: none;
    }
    
  }
}
</style>