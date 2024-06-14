<template>
  <v-card elevation="10" class="crs-card text-left rounded-xl bg-white">
    <v-card-item class="bg-white">
        <img src="@/assets/images/section3_img1.jpeg" alt="" class="course-img">
        <div class="div-ctn">
            <p class="card-title">Intro to Blockchain</p>
            <p class="card-text">Start with the basics of blockchain technology and its applications.</p>
            <ul>
                <li class="card-text">Duration: 4 weeks</li>
                <li class="card-text">Instructor: Jane Doe</li>
                <li class="card-text">Skill Level: Beginner</li>
            </ul>
            <v-btn color="#6366f1" variant="flat" class="py-6 px-3 btn">Learn More</v-btn>
        </div>
    </v-card-item>
  </v-card>
</template>

<script>
export default {

}
</script>

<style scoped>
.crs-card {
    overflow: hidden;
    padding: 4vh 2.2vw;
    background: #ffffff !important;
    color: #000000;
    cursor: pointer;
}
.course-img {
    width: auto;
    max-width: 100%;
    height: 100%;
    max-height: 30vh;
    border-radius: 10px 10px 0px 0px;
}
.div-ctn {
    color: #000000;
}
.crs-card p.card-title {
    color: #4f46e5;
    font-size: 1.6em;
    font-weight: bold;
}
.card-text {
    color: #374151;
    font-size: 16px;
}
ul {
    margin: 2vh 0 3vh;
}
.btn {
    font-weight: bold;
    text-transform: capitalize;
}
</style>