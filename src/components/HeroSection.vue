<template>
  <section class="pre-leader-board leader-board">
    <div class="container w-75">
      <div class="hero-section-content text-center">
        <img :src="pageData.image" :alt="pageData.subtitle" class="img-fluid">
        <h2 class="title text-uppercase">
          Salty<span class="primary-text">Ape</span>
        </h2>
        <h3>
          {{ pageData.subtitle }}
        </h3>
        <p class="text">
          {{ pageData.description }}
        </p>
        <p>
          <a href="#what">More Info...</a>
        </p>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref, onMounted } from 'vue'

// import { defineProps } from 'vue'
//   const props = defineProps({
//     msg: String
//   })

const pageData = ref(
  {
    title: 'Salty Ape',
    subtitle: 'Coming to you live from the interwebs',
    description: 'Salty Ape is more than a Vue Template.  Salty Ape is a lifestyle.  Salty Ape is a way of life.  Salty Ape is a way of being, a way of thinking, a way of believing.  But yeah, it\'s also a Vue Template.  So there\'s that. More specifically it\'s a Vue 3 SPA Template that uses Bootstrap instead of Tailwind CSS...',
    image: '/images/saltyApe2.webp',
    imageAlt: 'Salty Ape is Vue 3 Template',
  }
)

</script>