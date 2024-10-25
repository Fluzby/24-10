<template>
  <transition name="fade">
    <div v-if="isOpen" class="fixed inset-0 flex items-center justify-center bg-black bg-opacity-50 z-50">
      <div class="bg-white p-6 rounded-lg shadow-lg w-96">
        <h3 class="text-2xl font-bold mb-4 text-black">Contact Us</h3>
        <form @submit.prevent="submitForm">
          <div class="mb-4">
            <label class="block text-black">Name</label>
            <input v-model="name" type="text" class="w-full px-4 py-2 border rounded text-black" required />
          </div>
          <div class="mb-4">
            <label class="block text-black">Email</label>
            <input v-model="email" type="email" class="w-full px-4 py-2 border rounded text-black" required />
          </div>
          <div class="mb-4">
            <label class="block text-black">Phone Number</label>
            <input v-model="phone" type="tel" class="w-full px-4 py-2 border rounded text-black" required />
          </div>
          <button type="submit" class="w-full px-4 py-2 bg-yellow-500 text-black rounded hover:bg-yellow-400">
            Submit
          </button>
        </form>
        <button @click="close" class="mt-4 text-red-500">Close</button>
      </div>
    </div>
  </transition>
</template>

<script>
export default {
  data() {
    return {
      isOpen: false,
      name: '',
      email: '',
      phone: '',
    };
  },
  methods: {
    open() {
      this.isOpen = true;
    },
    close() {
      this.isOpen = false;
    },
    submitForm() {
      console.log('Submitted:', { name: this.name, email: this.email, phone: this.phone });
      this.close(); 
    },
  },
};
</script>

<style>
.fade-enter-active, .fade-leave-active {
  transition: opacity 1s ease-in-out;
}
.fade-enter, .fade-leave-to {
  opacity: 0; 
}
</style>
