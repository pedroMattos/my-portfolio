<template>
  <div>
    <banner-header></banner-header>
    <about-section></about-section>
    <skills-section></skills-section>
  </div>
</template>

<script>
import banner from '../components/header/banner.vue';
import aboutSection from '../components/About/section.vue'
import skillsSection from '../components/Skills/section.vue'

export default {
  name: 'home',
  components: {
    'banner-header': banner,
    'about-section': aboutSection,
    'skills-section': skillsSection
  },
};
</script>

<style lang="scss">
.chart {
  height: 400px;
}
</style>
