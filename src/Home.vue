<script setup>
// import { RouterView } from 'vue-router'
import Navbar from './components/Navbar.vue'
import Hero from './components/Hero.vue'
import Partners from './components/Partners.vue'
import WhoAreWe from './components/WhoAreWe.vue'
import WhatWeDo from './components/WhatWeDo.vue'
import OurVision from './components/OurVision.vue'
import OurMission from './components/OurMission.vue'
import AppsAndData from './components/AppsAndData.vue'
import GetInvolved from './components/GetInvolved.vue'
import Footer from './components/Footer.vue'
// import "./assets/styles/main.scss"
import "./assets/styles/App.scss"


// const routes = {
//   '/': Home,
//   '/about': About
// }

// export default {
//   data() {
//     return {
//       currentPath: window.location.hash
//     }
//   },
//   computed: {
//     currentView() {
//       return routes[this.currentPath.slice(1) || '/'] || NotFound
//     }
//   },
//   mounted() {
//     window.addEventListener('hashchange', () => {
//       this.currentPath = window.location.hash
//     })
//   }
// }

</script>

<template>
    <!-- <header> -->
    <!-- <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="125" height="125" /> -->

    <!-- <div class="wrapper"> -->
    <Navbar />
    <Hero />
    <Partners />
    <WhoAreWe />
    <WhatWeDo />
    <OurVision />
    <OurMission />
    <AppsAndData />
    <GetInvolved />
    <Footer />

    <!-- <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav> -->
    <!-- </div> -->
    <!-- </header> -->

    <!-- <RouterView /> -->
</template>


<style scoped></style>
