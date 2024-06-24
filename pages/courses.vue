<template>
  <v-row>
    <v-col cols="12">
        <Jumbotron :details="jumboInfo" />
    </v-col>
    <v-col cols="12">
        <ExploreCourses id="courses"/>
    </v-col>
  </v-row>
</template>

<script>
export default {
  name: 'CoursesPage',
  data() {
    return {
      jumboInfo: {
        herofirst: 'Explore',
        herosec: 'Our',
        herolast: 'Courses',
        detail: 'We offer a wide range of courses designed to help you master Web3 technologies with ease and confidence.',
        btnText: 'Start Learning',
        courses: true
      }
    }
  },
}
</script>

<style scoped>

</style>