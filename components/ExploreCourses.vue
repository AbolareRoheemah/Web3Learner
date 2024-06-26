<template>
  <v-container>
    <v-row class="explore-ctn">
        <v-col cols="12">
            <p class="sect4-header">Explore Our Premium Courses</p>
            <p class="sect4-subheader pb-8">Unlock your potential with our diverse range of web3 courses, crafted to guide you every step of the way.</p>
        </v-col>
        <v-col cols="12">
            <v-row>
              <template v-for="(course, index) in courses">
                <v-col cols="12" md="4" :key="index">
                  <v-hover v-slot="{ hover }">
                    <Course :details="course" :class="[hover ? 'scale-up': 'scale-down']" :hovering="hover" />
                  </v-hover>
                </v-col>
              </template>
            </v-row>
        </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      isHovering: false,
      courses: [
        {
          title: 'Intro to Blockchain',
          detail: 'Start with the basics of blockchain technology and its applications.',
          duration: '4 weeks',
          instructor: 'Jane Doe',
          level: 'Beginner',
          image: 'course-img1.jpg'
        },
        {
          title: 'Smart Contract Development',
          detail: 'Delve into the world of smart contracts and decentralized applications (dApps).',
          duration: '6 weeks',
          instructor: 'John Smith',
          level: 'Intermediate',
          image: 'course-img2.jpg'
        },
        {
          title: 'Advanced dApp Development',
          detail: 'Develop sophisticated decentralized applications using advanced techniques.',
          duration: '5 weeks',
          instructor: 'Jane Doe',
          level: 'Beginner',
          image: 'course-img3.jpg'
        },
        {
          title: 'Decentralized Finance (DeFi) Mastery',
          detail: 'Decentralized Finance (DeFi) Mastery',
          duration: '7 weeks',
          instructor: 'Jane Doe',
          level: 'Beginner',
          image: 'course-img4.jpg'
        },
        {
          title: 'Intro to NFTs',
          detail: 'Understand the fundamentals of non-fungible tokens (NFTs) and their uses.',
          duration: '3 weeks',
          instructor: 'Jane Doe',
          level: 'Beginner',
          image: 'course-img5.jpg'
        },
        {
          title: 'Blockchain Security',
          detail: 'Learn the best practices for ensuring the security of blockchain-based systems.',
          duration: '10 weeks',
          instructor: 'Jane Doe',
          level: 'Beginner',
          image: 'course-img6.jpg'
        },
        {
          title: 'Ethereum Development',
          detail: 'Build and deploy smart contracts on the Ethereum blockchain.',
          duration: '5 weeks',
          instructor: 'Jane Doe',
          level: 'Beginner',
          image: 'course-img7.jpg'
        },
        {
          title: 'AI & Blockchain',
          detail: 'Explore the intersection of artificial intelligence and blockchain technology.',
          duration: '6 weeks',
          instructor: 'Jane Doe',
          level: 'Beginner',
          image: 'course-img9.jpg'
        },
        {
          title: 'Web3 Marketing',
          detail: 'Gain skills in marketing strategies specifically for web3 projects.',
          duration: '4 weeks',
          instructor: 'Jane Doe',
          level: 'Beginner',
          image: 'course-img8.jpg'
        },
      ]
    }
  },
}
</script>

<style scoped>
.explore-ctn {
    background-color: #eef2ff;
    text-align: center;
    border-radius: 10px;
    /* box-shadow: 4px 4px #f3f4f6; */
    padding: 5vh 5vw 10vh;
    margin-bottom: 10vh;
}
.sect4-header {
  color: #000;
  font-size: 3em;
  font-weight: bolder;
  padding: 0;
  margin: 0;
}
.sect4-subheader {
  color: #6b7280;
  padding: 0;
  margin: 0;
}
</style>