<template>
  <div :class="['tooltip-content', positionFiltred]">
    <p class="centralizer">{{ mensagem }}</p>
  </div>
</template>

<script>
export default {
  name: 'my-tooltip',
  props: ['msg', 'position'],
  data() {
    return {
      mensagem: null,
      positionFiltred: '',
    }
  },
  mounted() {
    this.mensagem = this.msg
    let tooltips = document.getElementsByClassName('tooltip-content')
    tooltips.forEach(tp => {
      tp.parentNode.setAttribute('style', 'position:relative')
      tp.parentNode.classList.add('hovered')
    });

    switch (this.position) {
      case 'right':
        this.positionFiltred = this.position
        break;
      case 'left':
        this.positionFiltred = this.position
        break;
      case 'top':
        this.positionFiltred = this.position
        break;
      case 'bottom':
        this.positionFiltred = this.position
        break;
      default:
        this.positionFiltred = ''
        break;
    }
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
  &.bottom {
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
  }
  &.right {
    position: absolute;
    display: none;
    background-color: black;
    bottom: unset;
    top: 10%;
    left: unset;
    right: -130px;
    padding: 4px 6px;
    border-radius: 4px;
    &::after {
      position: absolute;
      content: '';
      width: 0;
      height: 0;
      border-top: 5px solid transparent;
      border-left: 5px solid transparent;
      border-bottom: 5px solid transparent;
      border-right: 5px solid black;
      bottom: 5px;
      // top: 0;
      // right: -10px;
      left: -10px;
    }
  }
  &.left {
    position: absolute;
    display: none;
    background-color: black;
    bottom: unset;
    top: 10%;
    left: -130px;
    right: unset;
    padding: 4px 6px;
    border-radius: 4px;
    &::after {
      position: absolute;
      content: '';
      width: 0;
      height: 0;
      border-top: 5px solid transparent;
      border-left: 5px solid black;
      border-bottom: 5px solid transparent;
      border-right: 5px solid transparent;
      bottom: 5px;
      // top: 0;
      right: -10px;
      // left: -10px;
    }
  }
  p {
    margin: 0;
    font-size: 11px !important;
    color: white !important;
  }
}
</style>
