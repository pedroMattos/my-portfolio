<template>
  <section class="banner center black">
    <div class="container">
      <br><br><br>
      <h2 class="centralizer no-bottom-m white">My Portfolio</h2>
      <div class="lines section-width"></div>
      <br>

      <div class="row c-portfolio">
        <div class="col-sm-12 col-md-4" v-for="(item, key) in dados" :key="key">
          <card-project :dataProp="item.dado"></card-project>
        </div>
      </div>
    </div>
    <br><br>
  </section>
</template>

<script>
import cardProjectVue from './card-project.vue'
export default {
  name: 'sectio-portfolio',
  components: {
    'card-project': cardProjectVue,
  },
  data() {
    return {
      dados: [
        {dado: 'G2R Empreendimentos',},
        {dado: 'G2R Empreendimentos',},
        {dado: 'G2R Empreendimentos',},
        {dado: 'G2R Empreendimentos',},
        {dado: 'G2R Empreendimentos',},
        {dado: 'G2R Empreendimentos',},
        {dado: 'G2R Empreendimentos',},
        {dado: 'G2R Empreendimentos',},
        {dado: 'G2R Empreendimentos',},
      ]
    }
  },
}
</script>
