<template>
    <section class="min-h-screen bg-gradient-to-b from-transparent via-black/80 to-black backdrop-blur-sm py-20">
      <div class="container mx-auto px-4">
        <!-- Header -->
        <div class="text-center mb-16" data-aos="fade-up">
          <h2 class="text-4xl font-bold text-white mb-4">Video Design</h2>
          <p class="text-gray-400 text-lg max-w-2xl mx-auto">
            Crafting captivating visual stories through dynamic video content and motion design
          </p>
        </div>
  
        <!-- Video Grid -->
        <div class="grid md:grid-cols-2 gap-8 max-w-6xl mx-auto mb-8">
          <!-- Video 1 -->
          <div class="video-card group cursor-pointer" data-aos="fade-right" @click="openVideoLink('https://www.tiktok.com/@fluzbyae/video/7436277652341804320')">
            <div class="relative overflow-hidden rounded-xl border border-white/30 bg-gradient-to-br from-white/10 to-black/30 backdrop-blur-sm">
              <video 
                class="w-full aspect-video object-cover rounded-xl transform group-hover:scale-105 transition-transform duration-500"
                autoplay
                loop
                muted
                playsinline
                @click.stop
              >
                <source src="/src/assets/Gt3rs_1.mp4" type="video/mp4">
                Your browser does not support the video tag.
              </video>
              <!-- Overlay with play icon -->
              <div class="absolute inset-0 bg-black/30 group-hover:bg-black/20 transition-all duration-300 flex items-center justify-center">
                <div class="opacity-0 group-hover:opacity-100 transition-opacity duration-300">
                  <svg xmlns="http://www.w3.org/2000/svg" class="h-12 w-12 text-white" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M14.752 11.168l-3.197-2.132A1 1 0 0010 9.87v4.263a1 1 0 001.555.832l3.197-2.132a1 1 0 000-1.664z" />
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 12a9 9 0 11-18 0 9 9 0 0118 0z" />
                  </svg>
                </div>
              </div>
              <!-- Video Info -->
              <div class="absolute bottom-0 left-0 right-0 p-6 bg-gradient-to-t from-black/80 to-transparent">
                <h3 class="text-xl font-semibold text-white mb-2">Gt3/rs</h3>
                <p class="text-gray-300 text-sm">Motion Graphics • Visual Effects • 2024</p>
              </div>
            </div>
          </div>
  
          <!-- Video 2 -->
          <div class="video-card group cursor-pointer" data-aos="fade-left" @click="openVideoLink('https://www.tiktok.com/@fluzbyae/video/7434681802624681')">
            <div class="relative overflow-hidden rounded-xl border border-white/30 bg-gradient-to-br from-white/10 to-black/30 backdrop-blur-sm">
              <video 
                class="w-full aspect-video object-cover rounded-xl transform group-hover:scale-105 transition-transform duration-500"
                autoplay
                loop
                muted
                playsinline
                @click.stop
              >
                <source src="/src/assets/RAAAAH.mp4" type="video/mp4">
                Your browser does not support the video tag.
              </video>
              <!-- Overlay with play icon -->
              <div class="absolute inset-0 bg-black/30 group-hover:bg-black/20 transition-all duration-300 flex items-center justify-center">
                <div class="opacity-0 group-hover:opacity-100 transition-opacity duration-300">
                  <svg xmlns="http://www.w3.org/2000/svg" class="h-12 w-12 text-white" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M14.752 11.168l-3.197-2.132A1 1 0 0010 9.87v4.263a1 1 0 001.555.832l3.197-2.132a1 1 0 000-1.664z" />
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 12a9 9 0 11-18 0 9 9 0 0118 0z" />
                  </svg>
                </div>
              </div>
              <!-- Video Info -->
              <div class="absolute bottom-0 left-0 right-0 p-6 bg-gradient-to-t from-black/80 to-transparent">
                <h3 class="text-xl font-semibold text-white mb-2">Opium Everest</h3>
                <p class="text-gray-300 text-sm">Animation • Color Grading • 2024</p>
              </div>
            </div>
          </div>
        </div>

        <!-- Video 3 (Below) -->
        <div class="grid grid-cols-1 gap-8 max-w-6xl mx-auto">
          <div class="video-card group cursor-pointer" data-aos="fade-up" @click="openVideoLink('YOUR_TIKTOK_URL_HERE')">
            <div class="relative overflow-hidden rounded-xl border border-white/30 bg-gradient-to-br from-white/10 to-black/30 backdrop-blur-sm">
              <video 
                class="w-full aspect-video object-cover rounded-xl transform group-hover:scale-105 transition-transform duration-500"
                autoplay
                loop
                muted
                playsinline
                @click.stop
              >
                <source src="/src/assets/IDOL.mp4" type="video/mp4">
                Your browser does not support the video tag.
              </video>
              <!-- Overlay with play icon -->
              <div class="absolute inset-0 bg-black/30 group-hover:bg-black/20 transition-all duration-300 flex items-center justify-center">
                <div class="opacity-0 group-hover:opacity-100 transition-opacity duration-300">
                  <svg xmlns="http://www.w3.org/2000/svg" class="h-12 w-12 text-white" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M14.752 11.168l-3.197-2.132A1 1 0 0010 9.87v4.263a1 1 0 001.555.832l3.197-2.132a1 1 0 000-1.664z" />
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 12a9 9 0 11-18 0 9 9 0 0118 0z" />
                  </svg>
                </div>
              </div>
              <!-- Video Info -->
              <div class="absolute bottom-0 left-0 right-0 p-6 bg-gradient-to-t from-black/80 to-transparent">
                <h3 class="text-xl font-semibold text-white mb-2">IDOL</h3>
                <p class="text-gray-300 text-sm">Motion Graphics • Visual Effects • 2023</p>
              </div>
            </div>
          </div>
        </div>
  
        <!-- Skills List -->
        <div class="mt-20 grid grid-cols-2 md:grid-cols-4 gap-6 max-w-4xl mx-auto text-center" data-aos="fade-up">
          <div class="p-4 rounded-lg bg-white/10 backdrop-blur-sm border border-white/20">
            <p class="text-white font-medium">Motion Graphics</p>
          </div>
          <div class="p-4 rounded-lg bg-white/10 backdrop-blur-sm border border-white/20">
            <p class="text-white font-medium">Visual Effects</p>
          </div>
          <div class="p-4 rounded-lg bg-white/10 backdrop-blur-sm border border-white/20">
            <p class="text-white font-medium">Color Grading</p>
          </div>
          <div class="p-4 rounded-lg bg-white/10 backdrop-blur-sm border border-white/20">
            <p class="text-white font-medium">3D Animation</p>
          </div>
        </div>
      </div>
    </section>
</template>

<script>
import AOS from 'aos';
import 'aos/dist/aos.css';

export default {
  name: 'VideoShowcase',
  mounted() {
    AOS.init({
      duration: 800,
      easing: 'ease-out',
      once: true
    });
  },
  methods: {
    openVideoLink(url) {
      window.open(url, '_blank');
    }
  }
};
</script>

<style scoped>
.video-card {
  transition: transform 0.3s ease-out;
}

.video-card:hover {
  transform: translateY(-8px);
}
</style>