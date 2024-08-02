<script setup>
import { ref } from 'vue';
import FstCard from "./components/Card1.vue"
import LyricsText from "./components/LyricsText.vue"
import LinksInfo from "./components/LinksInfo.vue"
const tabList = ref(1);
const edit =(num) =>
{
  tabList.value  = num; 
}
</script>
<template>
  <v-app>
    <v-main>
      <v-container>
        <v-tabs>
          <v-tab @click="edit(1)" >Track Information</v-tab>
          <v-tab  @click="edit(2)" >Lyrics</v-tab>
          <v-tab  @click="edit(3)" >Links</v-tab>
        </v-tabs>
        <div>
          <div v-if = "tabList === 1">
            <FstCard />
          </div>
          <LyricsText v-if = "tabList === 2"/>
          <LinksInfo v-if = "tabList === 3"/>

        </div>
      </v-container>  
    </v-main>
  </v-app>
</template>

