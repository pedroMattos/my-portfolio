<template>
  <div>
    <banner-header></banner-header>
    <about-section></about-section>
  </div>
</template>

<script>
import banner from '../components/header/banner.vue';
import aboutSection from '../components/About/section.vue'

export default {
  name: 'home',
  components: {
    'banner-header': banner,
    'about-section': aboutSection,
  },
};
</script>
