<template>
  <div class="jumbotron">
    <p class="slide-in-left" transition="slide-x-transition">Master <br>Web3 <br>Technologies</p>
    <p class="learn slide-in-bottom">Learn in-demand web3 languages and technologies quickly and effectively with hands-on projects.</p>
    <v-btn variant="flat" size="large" class="text-center py-5 jumb-btn" color="#6366f1">Get Started Today</v-btn>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.jumbotron {
  background-image: url("../assets/images/Section1_image.jpeg");
  background-size: cover;
  /* background-color: red; */
  background-repeat: no-repeat;
  width: 100vw;
  height: 90vh;
  padding: 20vh 0 15vh 15vw;
  color: #fff;
}
.jumbotron p:first-child {
  font-size: 5em;
  font-weight: bold;
  line-height: 85px;
}
.jumbotron p.learn {
  width: 37%;
  font-size: 1.3em;
}
.jumb-btn {
  color: #fff;
}
@media screen and (max-width: 768px) {
  .jumbotron {
    height: auto;
    padding: 20vh 5vw 15vh;
  }
  .jumbotron p.learn {
    width: 100%;
  }
}
@media screen and (max-width: 525px) {
  .jumbotron p:first-child {
    font-size: 3em;
    line-height: 60px;
  }
}
</style>