<template lang="">
  <ul class="movie-list list-group">
    <MovieListItem v-for="movie in movies" :movie="movie" />
  </ul>
</template>
<script>
import MovieListItem from "../movie-list-item/MovieListItem.vue";
export default {
  components: {
    MovieListItem,
  },
  data() {
    return {
      movies: [
        {
          name: "Omar",
          viewers: 811,
          favourite: true,
          like: false,
        },
        {
          name: "Empire of Osman",
          viewers: 511,
          favourite: false,
          like: false,
        },
        {
          name: "Ertugrul",
          viewers: 611,
          favourite: true,
          like: true,
        },
      ],
    };
  },
};
</script>
<style scoped>
.movie-list {
  margin-top: 2rem;
  padding: 1.5rem;
  background-color: #fcfaf5;
  border-radius: 4px;
  box-shadow: 15px 15px 15px rgba(0, 0, 0, 0.15);
}
</style>
