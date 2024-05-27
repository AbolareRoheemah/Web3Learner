<template>
  <div class="footer-ctn">
    <v-row>
        <v-col>
            <p class="logo">Web3Learner</p>
        </v-col>
    </v-row>
    <v-row class="justify-start align-center text-center">
        <v-col class="text-left">
            <p class="footer-txt">Learning Web3 technologies made ease, quick and highly effective.</p>
            <div class="socials">
                
            </div>
        </v-col>
        <v-col>
            <p class="footer-txt">Terms of Service</p>
            <p class="footer-txt">Privacy Policy</p>
        </v-col>
        <v-col>
            <p class="footer-txt">Lagos State, Nigeria</p>
            <p class="footer-txt">+234 123 456 7890</p>
            <p class="footer-txt">contact@web3learner.org</p>
        </v-col>
    </v-row>
    <v-row class="justify-center align-center text-center">
        <v-col>
            <p class="footer-txt">&copy; 2024 Web3Learner. All rights reserved.</p>
        </v-col>
    </v-row>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.footer-ctn {
    position: relative;
    bottom: 0;
    background: #eef2ff;
    padding: 10vh 6vw;
}
.footer-txt {
    color: #000;
}
.logo {
    color: #000;
    font-size: 1.3em;
    font-weight: bolder;
}
</style>