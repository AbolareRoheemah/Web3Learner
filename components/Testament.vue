<template>
    <div class="sect4-div">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--!Font Awesome Free 6.5.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free Copyright 2024 Fonticons, Inc.--><path fill="#a5b4fc" d="M448 296c0 66.3-53.7 120-120 120h-8c-17.7 0-32-14.3-32-32s14.3-32 32-32h8c30.9 0 56-25.1 56-56v-8H320c-35.3 0-64-28.7-64-64V160c0-35.3 28.7-64 64-64h64c35.3 0 64 28.7 64 64v32 32 72zm-256 0c0 66.3-53.7 120-120 120H64c-17.7 0-32-14.3-32-32s14.3-32 32-32h8c30.9 0 56-25.1 56-56v-8H64c-35.3 0-64-28.7-64-64V160c0-35.3 28.7-64 64-64h64c35.3 0 64 28.7 64 64v32 32 72z"/></svg>
        <div class="body">
        <div class="peeps">
            <img src="@/assets/images/section4_img.jpeg" alt="">
        </div>
        <div class="sect4-text pl-9">
            <p class="name">John Doe</p>
            <FiveStar />
            <p class="testament">This platform made learning web3 technologies easy and fun!</p>
        </div>
        </div>
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--!Font Awesome Free 6.5.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free Copyright 2024 Fonticons, Inc.--><path fill="#a5b4fc" d="M0 216C0 149.7 53.7 96 120 96h8c17.7 0 32 14.3 32 32s-14.3 32-32 32h-8c-30.9 0-56 25.1-56 56v8h64c35.3 0 64 28.7 64 64v64c0 35.3-28.7 64-64 64H64c-35.3 0-64-28.7-64-64V320 288 216zm256 0c0-66.3 53.7-120 120-120h8c17.7 0 32 14.3 32 32s-14.3 32-32 32h-8c-30.9 0-56 25.1-56 56v8h64c35.3 0 64 28.7 64 64v64c0 35.3-28.7 64-64 64H320c-35.3 0-64-28.7-64-64V320 288 216z"/></svg>
    </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.sect4-div {
  background: #fff;
  box-shadow: 10px solid #374151;
  position: relative;
  min-height: 30vh;
  border-radius: 20px;
  padding: 5vh 2vw;
  width: 100%;
  height: auto;
  min-height: 30vh;
  margin-left: auto;
  margin-right: auto;
}
.sect4-div > svg {
  width: 60px;
  position: absolute;
  color: #a5b4fc;
}
.sect4-div > svg:first-child {
 right: 2vw;
 top: -3.5vh;
}
.sect4-div > svg:last-child {
  left: 2vw;
  bottom: -3.5vh;
}
.peeps img{
  width: 80px;
  height: 80px;
  border-radius: 50%;
}
.name {
  color: #000;
  padding: 0%;
  margin: 0%;
}
.body {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: top;
}
.testament {
  color: #9ca3af;
  padding-top: 2vh;
}
.sect4-text {
  text-align: left;
}

/* @media screen and (max-width: 768px) {
  .sect4-div {
    margin-top: 3vh;
  }
} */
</style>