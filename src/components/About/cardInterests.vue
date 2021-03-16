<template>
  <div class="card-interests">
    <p class="centralizer">
      <game-pad></game-pad>
    </p>
    <p class="centralizer small">
      Games
    </p>
  </div>
</template>

<script>
import gamepad from '../../assets/svg/gamepad';
export default {
  name: 'card-interests',
  components: {
    'game-pad': gamepad
  }
}
</script>
