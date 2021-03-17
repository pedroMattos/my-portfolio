<template>
  <div class="banner center">
    <div class="text-banner">
      <h2 class="white centralizer no-bottom-m">Skills</h2>
      <div class="lines section-width"></div>
    </div>
    <div id="skills-graphics">
      <div class="row">
        <div class="col-sm-12 col-md-6">
          <front-skills></front-skills>
        </div>
        <div class="col-sm-12 col-md-6">
          <back-skills></back-skills>
        </div>
      </div>
    </div>
    <div class="overlay"></div>
    <img id="img-banner" src="@/assets/images/banner-skills.jpg" alt="Banner Home">
  </div>
</template>

<script>
import frontSkills from './graphSkillFront';
import backSkills from './graphSkillBack';
export default {
  name: 'section-skills',
  components: {
    'front-skills': frontSkills,
    'back-skills': backSkills
  }
}
</script>

<style lang="scss">
 #skills-graphics {
   position: absolute;
   z-index: 2;
   left: 0;
   right: 0;
   top: 30%;
 }
</style>
