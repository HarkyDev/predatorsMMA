<script setup>
import MainHero from "../components/Home/MainHero.vue"
import AboutSection from "../components/Home/AboutSection.vue"
import OfferedSection from "../components/Home/OfferedSection.vue"
import NavBar from "../components/home/NavBar.vue"
import TeamSection from "../components/Home/TeamSection.vue"
import ReviewsSection from "../components/Home/ReviewsSection.vue"
</script>

<template>
  <main>
    <NavBar />
    <MainHero />
    <Team-section />
    <About-section />
    <OfferedSection />
    <ReviewsSection />
  </main>
</template>
