<template>
  <div>
    <banner-header></banner-header>
    <h1>Base</h1>
    <h2>About</h2>
    <h3>Personal details</h3>
    <p class="bold"><span>Hello! I'm Pedro Mattos.</span> Lorem ipsum dolor sit amet,
      consectetur adipiscing elit, sed do eiusmod tempor
      incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud
      exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p>
    <p class="small">Lorem ipsum dolor sit amet</p>
  </div>
</template>

<script>
import banner from '../components/header/banner.vue';

export default {
  name: 'home',
  components: {
    'banner-header': banner,
  },
};
</script>
