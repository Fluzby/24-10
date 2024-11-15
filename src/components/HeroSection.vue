<template>
  <section class="relative h-screen bg-cover bg-center animate-fade-in" style="background-image: url('/src/assets/6227297.jpg')">
    <!-- Gradient overlay for transition -->
    <div class="absolute inset-0 bg-gradient-to-b from-transparent via-black/60 to-black pointer-events-none"></div>

    <div class="absolute top-8 left-1/2 transform -translate-x-1/2 z-20 flex items-center space-x-4">
      <span class="text-sm font-medium text-white">Oliver</span>

      <img src="/src/assets/logo.png" alt="Logo" class="h-50 w-60">
      
      <span class="text-sm font-medium text-white">P6der</span>
    </div>

    <div class="relative z-10 flex flex-col items-center justify-center h-full space-y-5">
      <h2 class="text-3xl text-white italic">Web Designer & Developer</h2>
      <p class="text-base text-gray-400">Specializing in Web Design, Development and Video Design</p>
      <button @click="$emit('open-popup')" class="mt-6 px-6 py-2 bg-white text-black rounded-lg hover:bg-gray-200 transition-colors duration-300">Let's Talk</button>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style>
@keyframes fadeIn {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}

.animate-fade-in {
  animation: fadeIn 2s ease-in-out;
}
</style>