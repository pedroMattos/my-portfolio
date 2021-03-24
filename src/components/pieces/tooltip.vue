<template>
  <div class="tooltip-content">
    <p class="centralizer">{{ mensagem }}</p>
  </div>
</template>

<script>
export default {
  name: 'my-tooltip',
  props: ['msg'],
  data() {
    return {
      mensagem: null
    }
  },
  mounted() {
    this.mensagem = this.msg
    let tooltips = document.getElementsByClassName('tooltip-content')
    tooltips.forEach(tp => {
      tp.parentNode.setAttribute('style', 'position:relative')
      tp.parentNode.classList.add('hovered')
    });
  },
}
</script>

<style lang="scss" scoped>
  .hovered {
    &:hover {
        .tooltip-content {
          display: block !important;
        }
    }
  }
.tooltip-content {
  position: absolute;
  display: none;
  background-color: black;
  bottom: -30px;
  left: 0;
  padding: 4px 6px;
  border-radius: 4px;
  &::after {
    position: absolute;
    content: '';
    width: 0;
    height: 0;
    border-top: 5px solid transparent;
    border-left: 5px solid transparent;
    border-bottom: 5px solid black;
    border-right: 5px solid transparent;
    bottom: 20px;
    // top: 0;
    // right: 0;
    left: 5px;
  }
  p {
    margin: 0;
    font-size: 11px !important;
  }
}
</style>
