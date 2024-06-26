<template>
  <v-card elevation="2" class="crs-card text-left rounded-xl bg-white mb-10">
    <v-card-item class="bg-white">
        <img :src="require(`@/assets/images/${details.image}`)" alt="" class="course-img" :class="[hovering ? 'img-hover': '']">
        <div class="div-ctn">
            <p class="card-title">{{details.title}}</p>
            <p class="card-text">{{details.detail}}</p>
            <ul>
                <li class="card-text">Duration: {{details.duration}}</li>
                <li class="card-text">Instructor: {{details.instructor}}</li>
                <li class="card-text">Skill Level: {{details.level}}</li>
            </ul>
            <!-- <v-btn color="blue-darken-4" variant="outlined" class="py-6 px-3 btn">Learn More</v-btn> -->
            <button class="btn" :class="{'btn-hover': hovering}">Learn More</button>
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
        hovering: {
            type: Boolean,
            default: () => false
        }
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
    /* box-shadow: #eef2ff; */
}
.course-img {
    width: auto;
    max-width: 100%;
    height: 100%;
    max-height: 30vh;
    border-radius: 10px 10px 0px 0px;
    opacity: 0.9;
    transition: opacity ease-in-out;
}
.img-hover {
    opacity: 1;
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
    font-weight: 500;
    color: #6366f1;
    text-transform: capitalize;
    border: 2px solid #6366f1;
    padding: 1vh 1vw;
    border-radius: 5px;
}
.btn-hover {
    background: #6366f1;
    border: none;
    color: #fff;
}
</style>