<template>
  <v-row>
    <v-col cols="12">
      <Jumbotron />
    </v-col> 
    <v-col cols="12">
      <HomeSectionTwo />
    </v-col>
    <v-col cols="12">
      <HomeSectionThree />
    </v-col>
    <v-col cols="12">
      <HomeSectionFour />
    </v-col>
    <v-col cols="12">
      <HomeSectionFive />
    </v-col>
  </v-row>
</template>

<script>
import Jumbotron from '../components/Jumbotron.vue'
export default {
  components: { Jumbotron },
  name: 'IndexPage'
}
</script>

<style scoped>
</style>