<template>
  <section class="container">
    <h2 class="centralizer no-bottom-m">About me</h2>
    <div class="lines section-width"></div>
    <br><br>
    <p><span>Hello! I'm Pedro Mattos.</span> Lorem ipsum dolor sit amet, consectetur
      adipiscing elit, sed do eiusmod tempor incididunt ut labore et
      dolore magna aliqua. Ut enim ad minim veniam, quis nostrud
      exercitation ullamco laboris nisi ut aliquip ex ea commodo
      consequat.</p>
      <br><br>
      <div class="row">
        <div class="col-sm-12 col-md-6">
          <personal-details></personal-details>
        </div>
        <div class="col-sm-12 col-md-6">
          <my-interests></my-interests>
        </div>
      </div>
      <br><br><br>
      <div class="row">
        <div class="col-sm-12">
          <btn-cta></btn-cta>
        </div>
      </div>
      <br><br>
  </section>
</template>

<script>
import peronalDetails from './personalDetails.vue';
import myInterests from './myInterests.vue';
import btnCta from '../../assets/cta/btnCta';

export default {
  name: 'section-about',
  components: {
    'personal-details': peronalDetails,
    'my-interests': myInterests,
    'btn-cta': btnCta,
  },
}
</script>
