<template>
  <div class="bg-black text-white min-h-screen">
    <HeroSection @open-popup="openPopup" />
    <Video />
    <AE />
    <FooterSection />  
    <ContactFormPopup ref="contactFormPopup" />
  </div>
</template>

<script>
import HeroSection from './components/HeroSection.vue';
import Video from './components/Video.vue'
import AE from './components/AE.vue'
import FooterSection from './components/FooterSection.vue';
import ContactFormPopup from './components/ContactFormPopup.vue';

export default {
  components: {
    HeroSection,
    Video,
    AE,
    FooterSection,
    ContactFormPopup,
  },
  methods: {
    openPopup() {
      this.$refs.contactFormPopup.open();
    },
  },
};
</script>

<style>
body {
  font-family: 'Consolas', 'Courier New';
}
</style>
