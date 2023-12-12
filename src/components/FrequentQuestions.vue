<template>
  <section class="faq" id="faq">
    <div class="container-fluid p-md-0">

      <div class="section-title text-center position-relative">
        <h6 class="small-title text-uppercase fs-7 fw-normal">FAQ</h6>
        <h2 class="title text-uppercase fw-bolder mb-10">FREQUENTLY <span class="primary-text">Asked Questions</span>
        </h2>
      </div>

      <div class="faq-wrapper">
        <div v-for="f in faq" key="i" class="item">
          <div class="faq-card-img-title d-md-flex align-items-center text-center text-md-start">
            <div class="faq-img flex-shrink-0">
              <img src="/images/faq.webp" alt="">
            </div>
            <h4 class="faq-title mb-0 fw-bold">
              {{f.question}}
            </h4>
          </div>
          <div class="faq-content-text">
            <p class="text mb-0">
              {{f.answer}}
            </p>
          </div>
        </div>
      </div>

    </div>

  </section>
</template>


<script setup>
import { onMounted, ref } from 'vue'
const faq = ref([
  {
    question: "How Can I Get This Code",
    answer: "Go to the download link above and that will take you to the Github repo.  You can clone it from there, and there is a README.md file with instructions."
  },
  {
    question: "Are You Available to hire?",
    answer: "Yes, I am available for hire.  I am a full stack developer with a focus on Vue 3, Node, and MongoDB.  I am also available for consulting and training.  Please contact me at ape@saltyape.com or txt: 850-270-3180"
  },
  {
    question: "How Can I Get on the Salty Ape Leader Board?",
    answer: "The Salty Ape Leader Board is a list of what's hot.  In Life.  If you have a link, topic, video, etc. that you want to share, please send it to ape@saltyape.com"
  },
  {
    question: "What is Bootstrap?",
    answer: "Bootstrap is the most popular HTML, CSS, and JS library in the world."
  }])


</script>