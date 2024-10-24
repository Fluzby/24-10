<template>
  <section class="relative h-screen bg-black text-center">
    <div class="relative z-10 flex flex-col items-center justify-center h-full space-y-5">
      <h1 class="text-4xl font-bold text-yellow-400">Oliver</h1> <!-- Changed from text-6xl to text-4xl -->
      <h2 class="text-3xl text-white italic">Web Designer & Developer</h2> <!-- Changed from text-5xl to text-3xl -->
      <p class="text-base text-gray-400">Specializing in Web Design, Development, and Video Design</p> <!-- Changed from text-lg to text-base -->
      <button @click="$emit('open-popup')" class="mt-6 px-6 py-2 bg-yellow-500 text-black rounded-lg hover:bg-yellow-400">Let’s Talk</button>
    </div>
  </section>
</template>

<script>
export default {};
</script>
