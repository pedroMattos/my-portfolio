<template>
  <div>
    <banner-header></banner-header>
    <about-section></about-section>
    <skills-section></skills-section>
    <history-section></history-section>
    <portfolio-section></portfolio-section>
  </div>
</template>

<script>
import banner from '../components/header/banner.vue';
import aboutSection from '../components/About/section.vue';
import skillsSection from '../components/Skills/section.vue';
import historySection from '../components/History/section.vue';
import portfolioSection from '../components/Portfolio/section.vue';

export default {
  name: 'home',
  components: {
    'banner-header': banner,
    'about-section': aboutSection,
    'skills-section': skillsSection,
    'history-section': historySection,
    'portfolio-section': portfolioSection,
  },
};
</script>

<style lang="scss">
.chart {
  height: 400px;
}
</style>
