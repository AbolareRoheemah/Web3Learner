<template>
  <v-row class="justify-center sect4-lee pt-10">
    <v-container>
      <v-col cols="12">
        <p class="sect4-header">What Our Learners Say</p>
        <p class="sect4-subheader">Hear from those who have transformed their careers with Web3Learner.</p>
      </v-col>
      <v-col cols="12" class="" md="">
        <v-row class="padd justify-space-between align-center mt-10">
          <v-col cols="4" lg="4" md="4" sm="6" class="bfor-sec4">
            <Testament image="@/assets/images/section4_img.jpeg"/>
          </v-col>
          <v-col cols="4" lg="4" md="4" sm="6">
            <Testament />
          </v-col>
          <v-col cols="4" lg="4" md="4" sm="6">
            <Testament />
          </v-col>
        </v-row>
      </v-col>
    </v-container>
  </v-row>
</template>

<script>
export default {

}
</script>

<style>
.sect4-lee {
  /* background-color: #eef2ff; */
  background: linear-gradient(180deg, #eef2ff 65%, #ffffff 100%);
  text-align: center;
  padding-bottom: 18vh;
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
.padd {
  padding: 0;
  display: flex;
  justify-content: space-between;
}
</style>