<template>
  <div class="footer-ctn">
    <v-container>
        <v-row>
            <v-col>
                <p class="logo">Web3Learner</p>
            </v-col>
        </v-row>
        <v-row class="roww justify-start align-lg-center align-md-top text-center">
            <v-col class="text-left coll">
                <p class="footer-txt">Learning Web3 technologies made ease, quick and highly effective.</p>
                <div class="socials mt-5">
                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 320 512"><!--!Font Awesome Free 6.5.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free Copyright 2024 Fonticons, Inc.--><path d="M80 299.3V512H196V299.3h86.5l18-97.8H196V166.9c0-51.7 20.3-71.5 72.7-71.5c16.3 0 29.4 .4 37 1.2V7.9C291.4 4 256.4 0 236.2 0C129.3 0 80 50.5 80 159.4v42.1H14v97.8H80z"/></svg>
                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512"><!--!Font Awesome Free 6.5.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free Copyright 2024 Fonticons, Inc.--><path d="M389.2 48h70.6L305.6 224.2 487 464H345L233.7 318.6 106.5 464H35.8L200.7 275.5 26.8 48H172.4L272.9 180.9 389.2 48zM364.4 421.8h39.1L151.1 88h-42L364.4 421.8z"/></svg>
                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--!Font Awesome Free 6.5.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free Copyright 2024 Fonticons, Inc.--><path d="M100.3 448H7.4V148.9h92.9zM53.8 108.1C24.1 108.1 0 83.5 0 53.8a53.8 53.8 0 0 1 107.6 0c0 29.7-24.1 54.3-53.8 54.3zM447.9 448h-92.7V302.4c0-34.7-.7-79.2-48.3-79.2-48.3 0-55.7 37.7-55.7 76.7V448h-92.8V148.9h89.1v40.8h1.3c12.4-23.5 42.7-48.3 87.9-48.3 94 0 111.3 61.9 111.3 142.3V448z"/></svg>
                </div>
            </v-col>
            <v-col class="coll">
                <p class="footer-txt">Terms of Service</p>
                <p class="footer-txt">Privacy Policy</p>
            </v-col>
            <v-col class="coll">
                <p class="footer-txt">Lagos State, Nigeria</p>
                <p class="footer-txt">+234 123 456 7890</p>
                <p class="footer-txt">contact@web3learner.org</p>
            </v-col>
        </v-row>
        <v-row class="justify-center align-center text-center copy">
            <v-col>
                <p class="footer-txt">&copy; 2024 Web3Learner. All rights reserved.</p>
            </v-col>
        </v-row>
    </v-container>
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
    padding: 10vh 0vw 5vh;
    color: #000;
}
.footer-txt {
    color: #000;
    cursor: pointer;
}
.logo {
    color: #000;
    font-size: 1.3em;
    font-weight: bolder;
}
.socials svg {
    width: 18px;
    height: 20px;
    margin-right: 1vw;
    cursor: pointer;
}
.copy {
    margin-top: 10vh;
}
@media screen and (max-width: 768px) {
    .roww {
      align-items: top;
    }
}
@media screen and (max-width: 540px) {
    .roww {
      flex-flow: wrap;
    }
    .roww > .coll {
        flex-basis: 50%;
    }
}
</style>