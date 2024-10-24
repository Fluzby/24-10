<template>
  <div class="bg-black text-white min-h-screen">
    <HeroSection @open-popup="openPopup" />
    <SkillsSection />
    <WorkSection />
    <ProcessSection />
    <FooterSection />  
    <ContactFormPopup ref="contactFormPopup" />
  </div>
</template>

<script>
import HeroSection from './components/HeroSection.vue';
import SkillsSection from './components/SkillsSection.vue';
import ProcessSection from './components/ProcessSection.vue';
import FooterSection from './components/FooterSection.vue';
import ContactFormPopup from './components/ContactFormPopup.vue';

export default {
  components: {
    HeroSection,
    SkillsSection,
    ProcessSection,
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
