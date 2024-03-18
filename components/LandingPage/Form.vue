<template>
  <section class="">
    <div class="container">
      <div class="row">
        <div class="col-sm-12">
          <div class="row">
            <div class="rmb-30 col-md-8">
              <h2 class="text-center text-md-left mb-3">Get a Quote Instantly</h2>
              <div>
                <div class="types">
                  <label class="checkbox-wrapper">Coverage-optimised WiFi +$1/sqm/mo
                    <input type="checkbox" v-model="coverageOptimized">
                    <span class="checkmark"></span>
                  </label>
                  <label class="checkbox-wrapper">Performance WiFi upgrade +$1/sqm/mo
                    <input type="checkbox" v-model="performanceUpgrade">
                    <span class="checkmark"></span>
                  </label>
                  <label class="checkbox-wrapper">Automatic power outage monitoring +$20/mo
                    <input type="checkbox" v-model="powerMonitoring">
                    <span class="checkmark"></span>
                  </label>
                  <label class="checkbox-wrapper">LTE internet backup +$50/mo
                    <input type="checkbox" v-model="lteBackup">
                    <span class="checkmark"></span>
                  </label>
                </div>
                <p class="square-meter">Square Meter</p>
                <div class="square">
                  <div class="square-number">{{ value }}</div>
                  <span>m<sup>2</sup></span>
                </div>
                <div class="ranges">
                  <div class="range-wrapper">
                    <b-form-input v-model="value" type="range" min="0" max="1000" size="lg"></b-form-input>
                  </div>
                  <div class="ranges-limits">
                    <div>0 m <sup>2</sup></div>
                    <div>1000 m <sup>2</sup></div>
                  </div>
                </div>

              </div>

            </div>
            <div class="col-md-4">
              <div class="xamin-blue-bg text-white px-3 py-5">
                <h3 class="text-white">Managed Network</h3>
                <p class="text-white m-0 mb-2">Router and managment</p>
                <span class="text-white price">${{total()}}/mo</span>
                <p class="text-white m-0">Competitors $3.20</p>
                <p class="text-white m-0 font-weight-bold">Top Features</p>
                <div class="list-item">
                  <img src="../../assets/images/home/mark.png" alt="icon">
                  <span>24/7 cloud monitoring</span>
                </div>
                <div class="list-item">
                  <img src="../../assets/images/home/mark.png" alt="icon">
                  <span>Multiple support channels</span>
                </div>
                <div class="list-item">
                  <img src="../../assets/images/home/mark.png" alt="icon">
                  <span class="">Same-day equipment replacement</span>
                </div>
                <div class=" text-center mt-5 w-100">
                  <a class="button white-btn button-icon w-100" href="#"><span class="btn-effect">Get Monthly Plan</span></a>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<script>

export default {
  name: 'Form',
  data() {
    return {
      defaultValue: 200,
      value: 0,
      coverageOptimized: true,
      performanceUpgrade: false,
      powerMonitoring: false,
      lteBackup: false,
    }
  },
  methods: {
    total() {
      return  +this.defaultValue + (+(this.coverageOptimized ? this.value : +0)) + (+(this.performanceUpgrade ? this.value : +0)) + (+(this.powerMonitoring ? +20 : +0)) + (+(this.lteBackup ? +50 : +0));
    }
  }
}
</script>
<style>
.checkbox-wrapper {
  display: block;
  position: relative;
  padding-left: 35px;
  margin-bottom: 12px;
  cursor: pointer;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

/* Hide the browser's default checkbox */
.checkbox-wrapper input {
  position: absolute;
  opacity: 0;
  cursor: pointer;
  height: 0;
  width: 0;
}

/* Create a custom checkbox */
.checkmark {
  position: absolute;
  top: 0;
  left: 0;
  height: 30px;
  width: 30px;
  background-color: #eee;
  border-radius: 15px;
}

/* On mouse-over, add a grey background color */
.checkbox-wrapper:hover input ~ .checkmark {
  background-color: #ccc;
}

/* When the checkbox is checked, add a blue background */
.checkbox-wrapper input:checked ~ .checkmark {
  background-color: #3F81D1;
}

/* Create the checkmark/indicator (hidden when not checked) */
.checkmark:after {
  content: "";
  position: absolute;
  display: none;
}

/* Show the checkmark when checked */
.checkbox-wrapper input:checked ~ .checkmark:after {
  display: block;
}

/* Style the checkmark/indicator */
.checkbox-wrapper .checkmark:after {
  left: 13px;
  top: 8px;
  width: 5px;
  height: 10px;
  border: solid white;
  border-width: 0 3px 3px 0;
  -webkit-transform: rotate(45deg);
  -ms-transform: rotate(45deg);
  transform: rotate(45deg);
}
  .price {
    display: block;
    width: 100%;
    text-align: center;
    background-color: #659ADA;
    font-weight: bold;
    border-radius: 3px;
    font-size: 30px;
    padding: 5px 0;
  }
  .list-item {
    display: flex;
    align-items: center;
    gap: 10px;
  }
  .square {
    display: flex;
    gap: 5px;
    align-items: center;
    margin-bottom: 10px;
    font-size: 21px;
  }
  .square-number {
    padding: 3px 30px;
    background-color: #EFF1FD;
    border: 1px solid #AAABB4;
  }
  .ranges {
    display: flex;
    flex-direction: column;
    max-width: 650px;
  }
  .ranges-limits {
    display: flex;
    justify-content: space-between;
  }
  .types {
    display: flex;
    flex-direction: column;
    gap: 23px;
    color: #343E59;
    font-size: 25px;
    font-style: normal;
    font-weight: 600;
    margin-bottom: 40px;
  }
  .square-meter {
    font-size: 20px;
  }
  @media (max-width: 601px) {
    .types {
      font-size: 18px;
      font-weight: 400;
    }
    .square-number {
      padding: 3px 50px;
    }
    .ranges {
      margin-top: 30px;
    }
  }
</style>
