<template>
  <div class="card-body">
    <div class="text-card">
      <p class="centralizer">{{ dataProp }}</p>
    </div>
    <img src="@/assets/images/g2r_apresentacao.png" :alt="dataProp" srcset="">
  </div>
</template>

<script>
export default {
  name: 'card-project',
  props: ['dataProp'],
}
</script>

<style lang="scss" scoped>
 .card-body {
   color: white;
 }
</style>
