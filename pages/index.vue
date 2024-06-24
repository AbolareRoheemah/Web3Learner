<template>
  <v-row>
    <v-col cols="12">
      <Jumbotron :details="jumboInfo"/>
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
  name: 'IndexPage',
  data() {
    return {
      jumboInfo: {
        herofirst: 'Master',
        herosec: 'Web3',
        herolast: 'Technologies',
        detail: 'Learn in-demand web3 languages and technologies quickly and effectively with hands-on projects.',
        btnText: 'Get Started Today',
        home: true
      }
    }
  },
}
</script>

<style scoped>
</style>