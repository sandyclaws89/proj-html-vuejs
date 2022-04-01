<template>
  <div id="app">
   <HeaderTeach />
   <MainTeach />
   <FooterTeach />
  </div>
</template>

<script>
import HeaderTeach from './components/HeaderTeach.vue'
import MainTeach from './components/MainTeach.vue'
import FooterTeach from './components/FooterTeach.vue'

export default {
  name: 'App',
  components: {
    HeaderTeach,
    MainTeach,
    FooterTeach
  }
}
</script>

<style lang="scss">
@import "@/assets/styles/style.scss";
// div{
// padding-bottom: 500px;
// }
</style>
