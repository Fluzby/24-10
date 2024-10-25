<template>
  <section class="py-10 bg-black">
    <div class="container mx-auto text-center">
      <h2 class="text-4xl font-bold text-white mb-6" data-aos="fade-up">My Skills</h2> 
      <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-8">
        <!-- All skill items will fade in at the same time -->
        <div class="skill-item bg-black p-6 rounded-lg shadow-lg border border-gray-700" data-aos="fade-up"> 
          <h3 class="text-2xl font-semibold text-white">Web Design</h3> 
          <p class="text-gray-400">Creating visually appealing and user-friendly designs.</p> 
        </div>
        <div class="skill-item bg-black p-6 rounded-lg shadow-lg border border-gray-700" data-aos="fade-up">
          <h3 class="text-2xl font-semibold text-white">Frontend Development</h3>
          <p class="text-gray-400">Building responsive and interactive user interfaces using HTML, CSS, and JavaScript.</p>
        </div>
        <div class="skill-item bg-black p-6 rounded-lg shadow-lg border border-gray-700" data-aos="fade-up"> 
          <h3 class="text-2xl font-semibold text-white">Backend Development</h3> 
          <p class="text-gray-400">Developing server-side applications and managing databases.</p> 
        </div>
        <div class="skill-item bg-black p-6 rounded-lg shadow-lg border border-gray-700" data-aos="fade-up"> 
          <h3 class="text-2xl font-semibold text-white">UX/UI Design</h3> 
          <p class="text-gray-400">Improving user experience through research and testing.</p> 
        </div>
        <div class="skill-item bg-black p-6 rounded-lg shadow-lg border border-gray-700" data-aos="fade-up"> 
          <h3 class="text-2xl font-semibold text-white">SEO Optimization</h3> 
          <p class="text-gray-400">Enhancing website visibility on search engines.</p> 
        </div>
        <div class="skill-item bg-black p-6 rounded-lg shadow-lg border border-gray-700" data-aos="fade-up"> 
          <h3 class="text-2xl font-semibold text-white">Project Management</h3> 
          <p class="text-gray-400">Coordinating and managing project timelines and deliverables.</p> 
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import AOS from 'aos';
import 'aos/dist/aos.css';

export default {
  mounted() {
    AOS.init({
      duration: 500, // Faster animation
      easing: 'ease-in-out', 
      once: true,
    });
  },
};
</script>

<style scoped>
.skill-item {
  transition: transform 0.3s;
}
.skill-item:hover {
  transform: translateY(-5px);
}
</style>
