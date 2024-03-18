<template>
  <section class="choose mt-5">
    <div class="container">
      <div class="choose-wrapper mt-5">
        <div class="choose-item" v-for="(list,index) in items" :key="index">
          <div class="">
            <span class="choose-title">{{list.title}}</span>
            <p class="choose-text">{{list.description}}</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  name: 'ChooseUs',
  data() {
    return {
      items: [
        {
          title: 'Zero upfront costs',
          description: 'Affordable running costs, aligned with your revenue model',
        },
        {
          title: 'Deployment and configuration',
          description: 'Most equipment wired, using professional equipment trusted by large enterprises',
        },
        {
          title: 'Professional network design & service',
          description: 'Giving you increased security, reliability and performance the best network is one you never notice',
        },
        {
          title: 'Single point of contact',
          description: 'Off-site and on-site top-down diagnosis in a timely manner system powered on, on-network, connection quality, actively transferring data, next steps',
        },
      ]
    }
  }
}
</script>
<style>
.choose-wrapper {
  min-height: 100%;
  display: flex;
  flex-wrap: wrap;
  flex-direction: row;
  justify-content: space-between;
}

.choose-item {
  display: flex;
  flex-basis: 40%;
  justify-content: center;
  flex-direction: column;
}

.choose-title {
  color: #3F81D1;
  font-size: 24px;
  font-weight: 400;
  margin-bottom: 10px;
}

.choose {
  padding-top: 0px;
}


.choose-text {
  color: #343E59;
  font-size: 20px;
  font-style: normal;
  margin-bottom: 50px;
}

@media only screen and (max-width: 600px) {
  .choose-wrapper {
    flex-direction: column;
  }
}

</style>
