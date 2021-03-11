<template>
  <div class="banner">
    <div class="text-banner">
      <h1 class="white centralizer">Pedro Mattos</h1>
      <div class="lines"></div>
      <h2 class="white centralizer">Code Designer</h2>
    </div>
    <avatar-photo></avatar-photo>
    <div class="overlay"></div>
    <img id="img-banner" src="@/assets/images/banner.jpg" alt="Banner Home">
  </div>
</template>

<script>
import avatar from './avatar.vue'

export default {
  name: 'banner',
  components: {
    'avatar-photo': avatar,
  },
}
</script>
