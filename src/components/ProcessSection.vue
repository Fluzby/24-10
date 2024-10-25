<template>
  <section class="bg-gray-800 py-12">
    <h2 class="text-center text-3xl font-semibold text-gray-300 mb-10" data-aos="fade-up">Different services I provide and the time period.</h2>
    <div class="max-w-6xl mx-auto space-y-8">
      <div class="flex items-start space-x-4" v-for="(step, index) in steps" :key="index" data-aos="fade-right" data-aos-delay="index * 100">
        <div class="w-2 bg-yellow-400 h-20"></div>
        <div>
          <h3 class="text-lg font-bold text-white">{{ step.title }}</h3>
          <p class="text-gray-400">{{ step.description }}</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import AOS from 'aos';
import 'aos/dist/aos.css';

export default {
  data() {
    return {
      steps: [
        { title: 'Discovery Call (30-60 min)', description: 'Let’s discuss your video concept, web design needs, or backend functionality to lay the groundwork for your project.' },
        { title: 'Video Design & Concept (1-2 week)', description: 'We’ll brainstorm and develop a creative direction for your video, ensuring it captures your message and vision with impactful visuals and storytelling.' },
        { title: 'Web Design (2 weeks)', description: 'Crafting a high-quality, responsive web design tailored to your brand’s aesthetic and user experience goals.' },
        { title: 'Backend Development (3-4 weeks)', description: 'Building robust backend architecture, including database design, API integration, and server-side functionality to support your website or web application.' },
        { title: 'Final Edits & Launch (2 hours)', description: 'Personalized walkthrough of the project, making final adjustments to your video, web design, and backend setup before launching it live.' }
      ]
    };
  },
  mounted() {
    AOS.init({
      duration: 500, // Speed up the animation duration
      easing: 'ease-in-out',
      once: true, // Animate only once
    });
  },
};
</script>

<style scoped>
/* No additional styles required for the animation since AOS handles it */
</style>
  