<template>
  <section class="no-margin-tp">
    <div class="container">
      <h2 class="centralizer no-bottom-m">My History</h2>
      <div class="lines section-width"></div>


      <br><br><br>
      <div class="history-map">
        <div class="container">
          <div class="row">
            <div class="col-md-6 right-border">
              <div class="card-history right">
                <div class="history-title">
                  <p>
                    Full-Stack Developer
                    <br>
                    <span class="subtitle">Ledax Energia Inteligente</span>
                  </p>
                </div>
                <div class="history-content">
                  <p>
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit,
                    sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
                  </p>
                </div>
              </div>
            </div>
            <div class="col-md-6 col-circle">
              <div class="circle">
                <div>
                  <check-svg></check-svg>
                  <m-tooltip msg="Jul/2020 - Till Today" position="right"></m-tooltip>
                </div>
              </div>
            </div>
          </div>

          <div class="row">
            <div class="col-md-6 right-border col-circle">
              <div class="circle right">
                <div>
                  <check-svg></check-svg>
                  <m-tooltip msg="Jun/2019 - Jun/2020" position="left"></m-tooltip>
                </div>
              </div>
            </div>
            <div class="col-md-6">
              <div class="card-history">
                <div class="history-title">
                  <p>
                    Full-Stack Developer
                    <br>
                    <span class="subtitle">Ledax Energia Inteligente</span>
                  </p>
                </div>
                <div class="history-content">
                  <p>
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit,
                    sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
                  </p>
                </div>
              </div>
            </div>
          </div>


          <div class="row">
            <div class="col-md-6 right-border">
              <div class="card-history right">
                <div class="history-title">
                  <p>
                    Full-Stack Developer
                    <br>
                    <span class="subtitle">Ledax Energia Inteligente</span>
                  </p>
                </div>
                <div class="history-content">
                  <p>
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit,
                    sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
                  </p>
                </div>
              </div>
            </div>
            <div class="col-md-6 col-circle">
              <div class="circle">
                <div>
                  <check-svg></check-svg>
                  <m-tooltip msg="Jun/2019 - Jun/2020" position="right"></m-tooltip>
                </div>
              </div>
            </div>
          </div>

          <div class="row">
            <div class="col-md-6 right-border col-circle">
              <div class="circle right">
                <div>
                  <check-svg></check-svg>
                  <m-tooltip msg="Jun/2019 - Jun/2020" position="left"></m-tooltip>
                </div>
              </div>
            </div>
            <div class="col-md-6">
              <div class="card-history">
                <div class="history-title">
                  <p>
                    Full-Stack Developer
                    <br>
                    <span class="subtitle">Ledax Energia Inteligente</span>
                  </p>
                </div>
                <div class="history-content">
                  <p>
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit,
                    sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
                  </p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <br><br><br>
  </section>
</template>

<script>
import checkVue from '../../assets/svg/check.vue'
import tooltipVue from '../pieces/tooltip.vue'
export default {
  name: 'section-history',
  components: {
    'check-svg': checkVue,
    'm-tooltip': tooltipVue,
  },
}
</script>
