<template>
  <section class="relative h-screen bg-cover bg-center animate-fade-in" style="background-image: url('/src/assets/apple-macbook-pro-stock-2021-apple-event-2021-dark-mode--6759.jpg')">
    <div class="relative z-10 flex flex-col items-center justify-center h-full space-y-5 bg-black bg-opacity-50">
      <h1 class="text-4xl font-bold text-yellow-400">Oliver</h1>
      <h2 class="text-3xl text-white italic">Web Designer & Developer</h2>
      <p class="text-base text-gray-400">Specializing in Web Design, Development, and Video Design</p>
      <button @click="$emit('open-popup')" class="mt-6 px-6 py-2 bg-yellow-500 text-black rounded-lg hover:bg-yellow-400">Let’s Talk</button>
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
