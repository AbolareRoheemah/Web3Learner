<template>
  <div class="jumbotron" :class="[details.home ? 'home' : details.courses ? 'courses': 'onecourse']">
    <!-- <p class="slide-in-left" transition="slide-x-transition">{{details.hero}}</p> -->
    <p class="slide-in-left" transition="slide-x-transition">{{details.herofirst}} <br class="d-xs-none d-print-block">{{details.herosec}} <br class="d-xs-none d-sm-print-block">{{details.herolast}}</p>
    <p class="learn slide-in-bottom">{{details.detail}}</p>
    <v-btn v-if="details.home" variant="flat" size="large" class="text-center py-5 jumb-btn" color="#6366f1" @click.prevent="$router.push('/courses')">{{details.btnText}}</v-btn>
    <a href="#courses" v-else><v-btn variant="flat" size="large" class="text-center py-5 jumb-btn" color="#6366f1">{{details.btnText}}</v-btn></a>
  </div>
</template>

<script>
export default {
  props: {
    details: {
      type: Object,
      default: () => {}
    },
  },
  methods: {
    // handlePush() {
    //   this.$router.push('/courses')
    // },
  },
}
</script>

<style scoped>
.jumbotron {
  background-size: cover;
  /* background-color: red; */
  background-repeat: no-repeat;
  width: 100vw;
  height: 90vh;
  padding: 20vh 0 15vh 15vw;
  color: #fff;
}
.home {
  background-image: url("../assets/images/Section1_image.jpeg");
}
.courses {
  background-image: url("../assets/images/courses.jpg");
}
.onecourse {
  background-image: url("../assets/images/courses.jpg");
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