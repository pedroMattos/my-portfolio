<template>
  <div>
    <h3>Personal Details</h3>
    <div class="row">
      <div class="col-md-3">
        <p class="small">Phone</p>
        <p class="small">Email</p>
        <p class="small">Address</p>
        <p class="small">Job Status</p>
      </div>
      <div class="col-md-6">
        <p class="small">+55 (71) 98535-1537</p>
        <p class="small">laranjeiraspedro@gmail.com</p>
        <p class="small">Salvador, BA - Brazil</p>
        <ul id="job-status">
          <li class="freelancer">Freelancer</li>
          <li class="ime">IME</li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'personal-details',
}
</script>
