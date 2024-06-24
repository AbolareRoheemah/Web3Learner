<template>
  <v-card elevation="10" class="crs-card text-left rounded-xl bg-white">
    <v-card-item class="bg-white">
        <img :src="require(`@/assets/images/${details.image}`)" alt="" class="course-img">
        <div class="div-ctn">
            <p class="card-title">{{details.title}}</p>
            <p class="card-text">{{details.detail}}</p>
            <ul>
                <li class="card-text">Duration: {{details.duration}}</li>
                <li class="card-text">Instructor: {{details.instructor}}</li>
                <li class="card-text">Skill Level: {{details.level}}</li>
            </ul>
            <v-btn color="#6366f1" variant="flat" class="py-6 px-3 btn">Learn More</v-btn>
        </div>
    </v-card-item>
  </v-card>
</template>

<script>
export default {
    props: {
        details: {
            type: Object,
            default: () => {}
        },
    },
}
</script>

<style scoped>
.crs-card {
    overflow: hidden;
    padding: 4vh 2.2vw;
    background: #ffffff !important;
    color: #000000;
    cursor: pointer;
    height: 80vh;
    max-height: 80vh;
}
.crs-card:hover {

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
    color: #fff;
    text-transform: capitalize;
}
</style>