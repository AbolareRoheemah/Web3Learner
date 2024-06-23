<template>
    <v-container>
      <v-row class="justify-center lee pt-10">
        <v-col cols="12">
          <p class="sect3-header">Our Courses Include</p>
        </v-col>
        <v-col cols="12" class="" md="">
          <div class="flx-ctn">
            <div @click="router.push('/courses')">
              <div class="sect3-div" @mouseover="isHovering1 = true" @mouseleave="isHovering1 = false">
                <img src="@/assets/images/section3_img1.jpeg" alt="" :class="isHovering1 ? 'scale-up': 'scale-down'">
                <p class="purplep" :class="isHovering1 ? 'p-hover': ''">Solidity For Beginners</p>
                <p class="sec3p">Dynamic and interactive learning modules to keep you engaged.</p>
              </div>
            </div>
            <div @click="router.push('/courses')">
              <div class="sect3-div" @mouseover="isHovering2 = true" @mouseleave="isHovering2 = false">
                <img src="@/assets/images/section3_img2.jpeg" alt="" :class="isHovering2 ? 'scale-up': 'scale-down'">
                <p class="purplep" :class="isHovering2 ? 'p-hover': ''">Learn Rust From Scratch</p>
                <p class="sec3p">Learn from industry leaders and top instructors in the field.</p>
              </div>
            </div>
            <div @click="router.push('/courses')">
              <div class="sect3-div" @mouseover="isHovering3 = true" @mouseleave="isHovering3 = false">
                <img src="@/assets/images/section3_img3.jpeg" alt="" :class="isHovering3 ? 'scale-up bright': 'scale-down'">
                <p class="purplep" :class="isHovering3 ? 'p-hover': ''">Building on Airdao</p>
                <p class="sec3p">Join a thriving community of web3 learners and builders worldwide.</p>
              </div>
            </div>
            <div @click="router.push('/courses')">
              <div class="sect3-div" @mouseover="isHovering4 = true" @mouseleave="isHovering4 = false">
                <img src="@/assets/images/section3_img4.jpeg" alt="" :class="isHovering4 ? 'scale-up': 'scale-down'">
                <p class="purplep" :class="isHovering4 ? 'p-hover': ''">Cairo: Smart Contract Development</p>
                <p class="sec3p">Hands-on projects that provide real-world experience.</p>
              </div>
            </div>
            <div @click="router.push('/courses')">
              <div class="sect3-div" @mouseover="isHovering5 = true" @mouseleave="isHovering5 = false">
                <img src="@/assets/images/section3_img5.jpeg" alt="" :class="isHovering5 ? 'scale-up': 'scale-down'">
                <p class="purplep" :class="isHovering5 ? 'p-hover': ''">Bitcoin Fundamentals</p>
                <p class="sec3p">Boost your career with in-demand web3 skills.</p>
              </div>
            </div>
            <div @click="router.push('/courses')">
              <div class="sect3-div" @mouseover="isHovering6 = true" @mouseleave="isHovering6 = false">
                <img src="@/assets/images/section3_img6.jpeg" alt="" :class="isHovering6 ? 'scale-up': 'scale-down'">
                <p class="purplep" :class="isHovering6 ? 'p-hover': ''">The Ethereum Blockchain</p>
                <p class="sec3p">Learn all about ethereum at your own pace with our flexible schedule options.</p>
              </div>
            </div>
            <div @click="router.push('/courses')">
              <div class="sect3-div" @mouseover="isHovering7 = true" @mouseleave="isHovering7 = false">
                <img src="@/assets/images/section3_img7.jpeg" alt="" :class="isHovering7 ? 'scale-up': 'scale-down'">
                <p class="purplep" :class="isHovering7 ? 'p-hover': ''">Smart Contract Devlopment</p>
                <p class="sec3p pt-0">Earn certificates that showcase your skills and knowledge.</p>
              </div>
            </div>
            <div @click="router.push('/courses')">
              <div class="sect3-div" @mouseover="isHovering8 = true" @mouseleave="isHovering8 = false">
                <img src="@/assets/images/section3_img8.jpeg" alt="" :class="isHovering8 ? 'scale-up': 'scale-down'">
                <p class="purplep" :class="isHovering8 ? 'p-hover': ''">Technical Writting in Web3</p>
                <p class="sec3p">Dynamic and interactive learning modules to keep you engaged.</p>
              </div>
            </div>
          </div>
        </v-col>
      </v-row>
    </v-container>
</template>

<script>
export default {
  data() {
    return {
      isHovering1: false,
      isHovering2: false,
      isHovering3: false,
      isHovering4: false,
      isHovering5: false,
      isHovering6: false,
      isHovering7: false,
      isHovering8: false
    }
  },
}
</script>

<style scoped>
.lee {
  background-color: white;
  padding: 0vh 0vw 6vh;
  margin-top: 10vh;
  max-width: 100vw;
}
.sect3-div {
  margin-bottom: 6vh;
  height: 45vh;
  max-height: 45vh;
}
.img-hover {
  transform: scale(1.1);
  transition: 1s;
}
.flx-ctn {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  flex-flow: wrap;
  gap: 10px;
}
.flx-ctn > div {
  flex-basis: 24%;
  overflow-y: hidden;
}
.sect3-header {
  font-size: 3em;
  font-weight: bolder;
  color: #000;
  margin: 0vh 0.5vw;
}
.p-hover {
  text-decoration: underline;
}
.sect3-div img {
  width: 99%;
  height: 25vh;
  max-height: 25vh;
  border-radius: 9px;
  cursor: pointer;
}
p.purplep {
  color: #4f46e5;
  font-weight: 600;
  padding: 2vh 0 0vh;
  cursor: pointer;
}
p.sec3p {
  color: #374151;
  font-weight: 500;
}
.bright {
  background-blend-mode: luminosity;
}
  @media screen and (max-width: 768px) {
    .flx-ctn {
        gap: 7px;
        justify-content: space-evenly;
    }
    .flx-ctn > div {
        flex-basis: 32%;
        height: auto;
        max-height: 60vh;
      }
      .sect3-header {
        margin: -5vh 0.5vw 0;
      }
  }
@media screen and (max-width: 699px) {
  .flx-ctn > div {
    flex-basis: 49%;
  }
}
@media screen and (max-width: 420px) {
  .flx-ctn > div {
    flex-basis: 100%;
  }
  .sect3-div {
    margin-bottom: 0;
  }
}
</style>