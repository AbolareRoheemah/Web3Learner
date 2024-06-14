<template>
  <v-container>
    <v-row class="explore-ctn">
        <v-col cols="12">
            <p class="sect4-header">Explore Our Premium Courses</p>
            <p class="sect4-subheader pb-8">Unlock your potential with our diverse range of web3 courses, crafted to guide you every step of the way.</p>
        </v-col>
        <v-col cols="12">
            <v-row>
                <v-col cols="4" v-for="(course, index) in [1, 2, 3, 4, 5, 6, 7, 8, 9]" :key="index">
                    <Course />
                </v-col>
            </v-row>
        </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {

}
</script>

<style scoped>
.explore-ctn {
    background-color: #f3f4f6;
    text-align: center;
    border-radius: 10px;
    box-shadow: 4px 4px #f3f4f6;
    padding: 5vh 5vw;
}
.sect4-header {
  color: #000;
  font-size: 3em;
  font-weight: bolder;
  padding: 0;
  margin: 0;
}
.sect4-subheader {
  color: #6b7280;
  padding: 0;
  margin: 0;
}
</style>