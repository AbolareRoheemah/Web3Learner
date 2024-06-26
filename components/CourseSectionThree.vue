<template>
    <v-container>
      <v-row class="justify-center lee pt-10">
        <v-col cols="12">
          <p class="sect3-header text-center">Course Modules</p>
        </v-col>
        <v-col cols="12" class="" md="">
          <div class="flx-ctn">
            <div @click="router.push('/courses')">
              <div class="sect3-div" @mouseover="isHovering1 = true" @mouseleave="isHovering1 = false">
                <img src="@/assets/images/section3_img4.jpeg" alt="" :class="isHovering1 ? 'scale-up opaque': 'scale-down'">
                <p class="purplep" :class="isHovering1 ? 'p-hover': ''">Introduction to web3</p>
                <p class="sec3p">DUnderstand the basics of Web3 and Blockchain technologies.</p>
              </div>
            </div>
            <div @click="router.push('/courses')">
              <div class="sect3-div" @mouseover="isHovering2 = true" @mouseleave="isHovering2 = false">
                <img src="@/assets/images/course-mod2.avif" alt="" :class="isHovering2 ? 'scale-up opaque': 'scale-down'">
                <p class="purplep" :class="isHovering2 ? 'p-hover': ''">Smart Contracts</p>
                <p class="sec3p">Learn how to create and deploy smart contracts using Solidity.</p>
              </div>
            </div>
            <div @click="router.push('/courses')">
              <div class="sect3-div" @mouseover="isHovering3 = true" @mouseleave="isHovering3 = false">
                <img src="@/assets/images/course-mod3.avif" alt="" :class="isHovering3 ? 'scale-up opaque': 'scale-down'">
                <p class="purplep" :class="isHovering3 ? 'p-hover': ''">Building Dapps</p>
                <p class="sec3p">Develop and interact with decentralized applications.</p>
              </div>
            </div>
            <div @click="router.push('/courses')">
              <div class="sect3-div" @mouseover="isHovering4 = true" @mouseleave="isHovering4 = false">
                <img src="@/assets/images/course-mod4.jpg" alt="" :class="isHovering4 ? 'scale-up opaque': 'scale-down'">
                <p class="purplep" :class="isHovering4 ? 'p-hover': ''">Advanced Blockchain Concepts</p>
                <p class="sec3p">Dive deeper into advanced concepts and frameworks in blockchain technology.</p>
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
  height: 65vh;
  max-height: 65vh;
  overflow: hidden;
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
  height: 47vh;
  max-height: 47vh;
  border-radius: 9px;
  cursor: pointer;
  opacity: 0.9;
}

.sect3-div .opaque {
  opacity: 1;
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