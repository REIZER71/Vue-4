<script>
  export default {
    data: () => ({
      items: Array.from({ length: 144 }, (k, v) => v + 1),
    }),
  }
</script>
<template>
     <v-card-item class="bg-black">
      <v-card-title>
       Lyrics
      </v-card-title>
      </v-card-item>
    <v-divider></v-divider>
    <br>
  <v-virtual-scroll  variant="outlined" :items="items" height="400">
    <template v-slot:default="{ item }">
        Around the world, around the world
    </template>
  </v-virtual-scroll>
</template>
