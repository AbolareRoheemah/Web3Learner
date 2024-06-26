<template>
    <div class="detail-ctn">
        <v-row>
            <v-col cols="12">
                <Jumbotron :details="jumboInfo" />
            </v-col>
            <v-col cols="12">
                <CourseSectionTwo />
            </v-col>
            <v-col cols="12">
                <CourseSectionThree />
            </v-col>
        </v-row>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                jumboInfo: {
                    hero: 'Explore',
                    detail: 'We offer a wide range of courses designed to help you master Web3 technologies with ease and confidence.',
                    btnText: 'Enroll Now',
                    indiv: true,
                }
            }
        },
    }
</script>

<style scoped>

</style>