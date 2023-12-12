<script setup>
import Header from './components/TheHeader.vue'
import HeroSection from './components/HeroSection.vue'
import DataTable from './components/DataTable.vue'
import TriStories from './components/TriStories.vue'
import CallToAction from './components/CallToAction.vue'
import LeadStory from './components/LeadStory.vue'
import FrequentQuestions from './components/FrequentQuestions.vue'
import Footer from './components/TheFooter.vue'
</script>

<template>
  <Header />
  <section class="site-content">
    <HeroSection />
    <DataTable />
    <TriStories />
    <CallToAction />
    <LeadStory />
    <FrequentQuestions />
  </section>
  <Footer />
</template>
