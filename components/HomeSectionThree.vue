<template>
    <v-container>
      <v-row class="justify-center lee pt-10">
        <v-col cols="12">
          <p class="sect3-header">Our Courses Include</p>
        </v-col>
        <v-col cols="12" class="" md="">
          <v-row>
            <v-col cols="3" lg="3" md="4" sm="6">
              <div class="sect3-div">
                <img src="@/assets/images/section3_img1.jpeg" alt="">
                <p class="purplep">Solidity For Beginners</p>
                <p class="sec3p">Dynamic and interactive learning modules to keep you engaged.</p>
              </div>
            </v-col>
            <v-col cols="3" lg="3" md="4" sm="6">
              <div class="sect3-div">
                <img src="@/assets/images/section3_img2.jpeg" alt="">
                <p class="purplep">Learn Rust From Scratch</p>
                <p class="sec3p">Learn from industry leaders and top instructors in the field.</p>
              </div>
            </v-col>
            <v-col cols="3" lg="3" md="4" sm="6">
              <div class="sect3-div">
                <img src="@/assets/images/section3_img3.jpeg" alt="">
                <p class="purplep">Building on Airdao</p>
                <p class="sec3p">Join a thriving community of web3 learners and builders worldwide.</p>
              </div>
            </v-col>
            <v-col cols="3" lg="3" md="4" sm="6">
              <div class="sect3-div">
                <img src="@/assets/images/section3_img4.jpeg" alt="">
                <p class="purplep">Cairo: Smart Contract Development</p>
                <p class="sec3p">Hands-on projects that provide real-world experience.</p>
              </div>
            </v-col>
            <v-col cols="3" lg="3" md="4" sm="6">
              <div class="sect3-div">
                <img src="@/assets/images/section3_img5.jpeg" alt="">
                <p class="purplep">Bitcoin Fundamentals</p>
                <p class="sec3p">Boost your career with in-demand web3 skills.</p>
              </div>
            </v-col>
            <v-col cols="3" lg="3" md="4" sm="6">
              <div class="sect3-div">
                <img src="@/assets/images/section3_img6.jpeg" alt="">
                <p class="purplep">The Ethereum Blockchain</p>
                <p class="sec3p">Learn all about ethereum at your own pace with our flexible schedule options.</p>
              </div>
            </v-col>
            <v-col cols="3" lg="3" md="4" sm="6">
              <div class="sect3-div">
                <img src="@/assets/images/section3_img7.jpeg" alt="">
                <p class="purplep">Smart Contract Devlopment</p>
                <p class="sec3p pt-0">Earn certificates that showcase your skills and knowledge.</p>
              </div>
            </v-col>
            <v-col cols="3" lg="3" md="4" sm="6">
              <div class="sect3-div">
                <img src="@/assets/images/section3_img8.jpeg" alt="">
                <p class="purplep">Technical Writting in Web3</p>
                <p class="sec3p">Dynamic and interactive learning modules to keep you engaged.</p>
              </div>
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
.lee {
  background-color: white;
  padding: 0vh 0vw 6vh;
  margin-top: 10vh;
}
.sect3-div {
  margin-bottom: 6vh;
}
.sect3-header {
  font-size: 3em;
  font-weight: bolder;
  color: #000;
  margin: 0vh 0.5vw;
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
</style>