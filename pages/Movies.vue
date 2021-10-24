<template>
  <div>
      <!-- using our nav bar component -->
      <Navbar/>
    <b-card>
      <b-col cols="12" sm="6" md="3">
           <!-- using our data component to display our data from the API -->
        <DataComp :movie-data="movieData" />
      </b-col>
    </b-card>
  </div>
</template>
<script>
export default {
    //storing movie data inside of an array
  data() {
    return {
      movieData: [],
    };
  },
  //Making an Api call
  async fetch() {
    this.movieData = await fetch(
      "http://www.omdbapi.com/?i=tt3896198&apikey=50cccd0b"
    ).then((res) => res.json());
  },
};
</script>