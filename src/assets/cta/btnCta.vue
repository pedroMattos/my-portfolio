<template>
  <div class="button-cta">
    <p class="centralizer">
      Download CV
    </p>
  </div>
</template>

<script>
export default {
  name: 'call-to-action',

  mounted() {
    let btn = document.getElementsByClassName('button-cta')[0]
    btn.addEventListener('mouseenter', () => {
      btn.classList.add('enter')
    })
    btn.addEventListener('mouseout', () => {
      btn.classList.remove('enter')
      btn.classList.add('out')
      setTimeout(() => {
        btn.classList.remove('out')
      }, 500);
    })
  },
}
</script>
