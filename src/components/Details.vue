<template>

  <div class="details col-8 yellow">
    <h1>{{movie.title}}</h1>
    <div class="row">
      <div class="col-7">
        <img :src="'https://image.tmdb.org/t/p/w500/' + movie.poster_path" alt="">
      </div>
      <div class="col-5">
        <h4>{{movie.release_date}}</h4>
        <h4>{{movie.overview}}</h4>
      </div>
    </div>
  </div>

</template>

<script>
  export default {
    name: 'Details',
    props: ['movie'],
    data() {
      return {
      }
    },
    computed: {},
    methods: {}

  }

</script>

<style>
  .yellow {
    background-color: yellow
  }
</style>