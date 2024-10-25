<template>
  <section class="bg-gray-900 py-16">
    <h2 class="text-center text-3xl font-semibold text-gray-300 mb-16" data-aos="fade-up">
      Different services I provide and the time period.
    </h2>
    <div class="max-w-7xl mx-auto relative">
      <div v-for="(step, index) in steps" :key="index" class="relative flex" :class="index % 2 === 0 ? 'flex-row-reverse' : 'flex-row'">
        
        <!-- Vertical Line -->
        <div class="absolute top-0 left-1/2 w-1 h-full bg-gray-700 transform -translate-x-1/2"></div>
        
        <!-- Step Content (Right for even, Left for odd) -->
        <div v-if="index % 2 === 0" class="w-1/2 flex justify-end pr-10">
          <div class="bg-gray-800 p-6 rounded-lg shadow-lg text-right w-96" 
               data-aos="fade-left" 
               :data-aos-delay="index * 100">
            <h3 class="text-xl font-bold text-white">{{ step.title }}</h3>
            <p class="text-gray-400">{{ step.description }}</p>
            <p class="text-sm text-gray-500 mt-2">{{ step.time }}</p>
          </div>
        </div>
        
        <!-- Dots -->
        <div class="w-10 h-10 bg-yellow-500 rounded-full flex items-center justify-center text-lg font-bold text-black z-10 relative transform translate-x-16">
          {{ index + 1 }}
        </div>
        
        <!-- Step Content (Left for odd, Right for even) -->
        <div v-if="index % 2 !== 0" class="w-1/2 flex justify-start pl-10">
          <div class="bg-gray-800 p-6 rounded-lg shadow-lg text-left w-96" 
               data-aos="fade-right" 
               :data-aos-delay="index * 100">
            <h3 class="text-xl font-bold text-white">{{ step.title }}</h3>
            <p class="text-gray-400">{{ step.description }}</p>
            <p class="text-sm text-gray-500 mt-2">{{ step.time }}</p>
          </div>
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
        { title: 'Discovery Call', description: 'Let’s discuss your video concept, web design needs, or backend functionality to lay the groundwork for your project.', time: '30-60 min' },
        { title: 'Concept & Strategy', description: 'Together we develop a strategy that successfully combines your goals, based on your target audience’s needs.', time: '1 Week' },
        { title: 'Web Design', description: 'Crafting a high-end design tailored to your brand’s aesthetic and user experience goals.', time: '1 Week' },
        { title: 'Development', description: 'In this step, I create a custom-built website using a modular web design system and CMS integration.', time: '3 Weeks' },
        { title: 'Website Onboarding', description: 'I’ll show you how to make changes to your new website and guide you through the final stages.', time: '2 Hours' },
      ],
    };
  },
  mounted() {
    AOS.init({
      duration: 500, 
      easing: 'ease-in-out',
      once: true, 
    });
  },
};
</script>

<style scoped>
.relative {
  position: relative;
}

.bg-gray-800 {
  background-color: #1f1f1f;
}

.bg-gray-900 {
  background-color: #181818;
}

.shadow-lg {
  box-shadow: 0 10px 15px rgba(0, 0, 0, 0.1);
}

.flex {
  display: flex;
  align-items: center;
}

.w-1 {
  width: 0%;
}

.w-96 {
  width: 24rem;
}

.pl-10 {
  padding-left: 2.5rem;
}

.pr-10 {
  padding-right: 2.5rem;
}

.text-right {
  text-align: right;
}

.text-left {
  text-align: left;
}

.absolute {
  position: absolute;
}

.text-center {
  text-align: center;
}

.bg-yellow-500 {
  background-color: #facc15;
}

.rounded-lg {
  border-radius: 0.5rem;
}

/* Added for circle positioning */
.transform {
  transform: translateX(1rem); /* Adjust this value to move closer to the right */
}
</style>
