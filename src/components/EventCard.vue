<template>
  <div class="card flex">
      <div class="date">{{CardDate}}</div>
      <div class="flex text">
            <h3>{{CardTitle}}</h3>
            
      </div>
  </div>
</template>

<script>
export default {
    name:'EventCard',
    props: {
        CardTitle: String,

    }
}
</script>

<style lang="scss">
    .card{
        background-color: rebeccapurple;
    }
</style>