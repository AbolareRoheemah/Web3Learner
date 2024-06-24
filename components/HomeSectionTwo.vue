<template>
    <v-row class="justify-center lee" ref="two">
        <v-col cols="5" class="sec2-img-ctn" :class="key ? 'visible': ''">
          <div class="before">
            <div class="sec2-img"></div>
          </div>
          <!-- <img src="@/assets/images/section2_image.jpeg" alt="" class="sec2-img"> -->
        </v-col>
        <v-col>
          <div class="sec2-text-ctn">
            <p class="why">Why Choose Web3Learner?</p>
            <p class="faded-text mb-5">At Web3Learner, we specialize in providing comprehensive and up-to-date training in the world of web3. Our platform is designed to make learning both accessible and engaging.</p>
            <p class="faded-text">With our tailored learning paths, you can acquire and practise the skills that are in demand in today's job market. Our hands-on projects ensure that you not only understand the theory but also get practical experience.</p>
            <ul class="sec2list mt-5">
              <li>Expert-curated courses</li>
              <li>Real-world projects</li>
              <li>Real-world projects</li>
              <li>Community support</li>
            </ul>
          <v-btn variant="flat" size="x-large" class="text-center mt-10 btn" color="#6366f1" @click="$router.push('/courses')">Join Us Now</v-btn>
          </div>
        </v-col>
    </v-row>
</template>

<script>
export default {
  data() {
    return {
      key: false
    }
  },
  // computed: {
  //   isVisible(el) {
  //     const {top, left, bottom, right} = el.getBoun
  //     const {innerWidth, innerHeight} = window
  //     return ((top > 0 && top < innerHeight) || (bottom > 0 && bottom < innerHeight) || (left > 0 && left < innerWidth) || (right > 0 && right < innerWidth)) 
  //   },
  // },
  methods: {
    isVisible(el) {
      const {top, left, bottom, right} = el.getBoundingClientRect()
      const {innerWidth, innerHeight} = window
      if ((top > 0 && top < innerHeight) || (bottom > 0 && bottom < innerHeight) || (left > 0 && left < innerWidth) || (right > 0 && right < innerWidth)) {
        this.key = true
      } else {
        this.key = false
      }
    },
  },
  Created () {
    isVisible(el)
  }
}
</script>

<style scoped>
.lee {
  background-color: white;
  padding: 0 6vw;
  widows: 100vw;
}
.sec2-text-ctn {
  /* color: #000; */
  padding: 7vh 5vw 4vh 5vw;
  height: auto;
  width: 50vw;
  height: auto;
  background: #fff;
}
.before {
  height: 80vh;
  width: 35vw;
  background-color: #eef2ff;
  position: relative;
  top: 0;
  left: -6vw;
  border-radius: 0% 10% 0% 20%;
}
.sec2-img {
  background-image: url("../assets/images/section2_image.jpeg");
  background-size: cover;
  background-position: bottom;
  height: 80vh;
  width: 35vw;
  position: absolute;
  top: 10vh;
  left: 7vw;
  border-radius: 20% 10%;
}
p.why {
  font-size: 2.7em;
  font-weight: 700;
  color: #000;
}
p.faded-text {
  color: #6b7280;
  font-size: 1.4em;
}
.sec2list {
  font-size: 1.2em;
  /* font-weight: bold; */
}
.visible {
  display: none;
}
.btn {
  color: #fff;
}
@media screen and (max-width: 768px) {
  .lee {
    padding: 0;
  }
  .sec2-img-ctn {
      display: none;
  }
  .sec2-text-ctn {
    width: 100%;
    max-width: 100vw;
    overflow: hidden;
    margin-left: 0;
  }
  p.faded-text {
    width: inherit;
    max-width: 90vw;
  }
}
</style>