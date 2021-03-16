<template>
  <div>
    <h3>My interests</h3>
    <br>
    <div class="row">
      <div class="col-md-2">
        <card-interests></card-interests>
      </div>
      <div class="col-md-2">
        <card-interests></card-interests>
      </div>
      <div class="col-md-2">
        <card-interests></card-interests>
      </div>
      <div class="col-md-2">
        <card-interests></card-interests>
      </div>
    </div>
    <br>
    <div class="row">
      <div class="col-md-2">
        <card-interests></card-interests>
      </div>
      <div class="col-md-2">
        <card-interests></card-interests>
      </div>
      <div class="col-md-2">
        <card-interests></card-interests>
      </div>
      <div class="col-md-2">
        <card-interests></card-interests>
      </div>
    </div>
  </div>
</template>

<script>
import cardInterests from './cardInterests';
export default {
  name: 'my-interests',
  components: {
    'card-interests': cardInterests,
  }
}
</script>
