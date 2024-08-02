<script>
  export default {
    data: () => ({
      rating: 4,
    }),
  }
</script>
<template>
    <v-card
      class="cards"
      color="black"
      elevation="40"
      margin="20"
    >
      <div class="d-flex justify-between">
        <v-card-title class="flex-grow-1 flex-column align-start">
          <div class="text-h5">
            <h2 class = "header">Around The World</h2>
          </div>
          <div class="text-h6 font-weight-thin">Daft Punk</div>
  
          <div class="text-h6 font-weight-thin">(1997)</div>
        </v-card-title>
  
        <v-img
          class="flex-grow-0"
          height="125px"
          src="https://i.scdn.co/image/ab67616d0000b2738ac778cc7d88779f74d33311"
          style="flex-basis: 125px"
          contain
        ></v-img>
      </div>
  
      <v-divider></v-divider>
  
      <v-card-actions class="pa-4">
        Rating:
  
        <v-spacer></v-spacer>
  
        <span class="text-grey-lighten-2 text-caption me-2">
          ({{ rating }})
        </span>
  
        <v-rating
          v-model="rating"
          active-color="yellow-accent-4"
          color="white"
          size="18"
          readonly
          hover
        ></v-rating>
      </v-card-actions>
    </v-card>
  </template>
  <style>
.cards{
    border: 10px;
    margin: 20px;
    border-radius: 40;
}
.header{
  color: red;
  text-shadow:
    1px 1px 1px black,
    2px 2px 1px yellow;
}
</style>