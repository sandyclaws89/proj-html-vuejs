<template>
  <section class="flex main-container news-card">
        <img :src="NewsImg" :alt="NewsTitle">
        <div>
            <span>ICN</span>
            <span>{{NewsData}}</span>
            <span>ICN</span>
            <span>{{NewsAuthor}}</span>
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
    }
}
</script>

<style lang="scss">
    .news-card{
        flex-direction: column;
        width: calc(90vw/3);
        span{
            padding: 7px;
        }
    }
</style>