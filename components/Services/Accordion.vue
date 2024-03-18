<template>
  <section>
    <div class="container">
      <div class="row">
        <div class="col-sm-12">
          <div class="iq-accordion career-style about-style">
            <div v-for="(item,index) in items" :key="index" class="iq-accordion-block">
              <div class="active-faq clearfix">
                <div class="container">
                  <div class="row ">
                    <div class="col-md-12 col-sm-12">
                      <a href="javascript:void(0)" class="accordion-title"><span>{{ item.title }}</span></a>
                    </div>
                  </div>
                </div>
              </div>
              <div class="accordion-details">
                <div class="container">
                  <div class="row mt-4 w-100  ml-4">
                    <p class="accordion-description">{{item.description}}</p>
                  </div>
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
  name: 'Accordion',
  data() {
    return {
      items: [
        {
          title: 'Why is my WiFi/internet slow?',
          description: 'Your slow experience may stem from WiFi congestion or limited Access Point coverage. Alternatively, the service you are using may be overloaded, in a different geographic region, or there is congestion in the internet service provider or international links.',
        },
        {
          title: 'How can I improve WiFi/internet speed?',
          description: 'To optimize your WiFi, move your device and Access Point nearer, or add Access Points to increase strong-signal coverage.',
        },
        {
          title: 'What differentiates wifiOne’s site WiFi design?',
          description: 'wifiOne tailors site WiFi to match customer objectives—whether it\'s providing seamless coverage for video calls, high capacity for media tasks, or optimizing for cost-efficiency. We then apply specialized algorithms to select the most suitable enterprise equipment and locations, deploying our bespoke mounting solution for a clearer signal.',
        },
        {
          title: 'What equipment does wifiOne use?',
          description: 'wifiOne uses only US and EU enterprise-grade equipment for active network elements. Where possible, we incorporate a capacity overprovision, ensuring redundancy against device failures and ample performance during peak times.\n All equipment is validated for enterprise use for continuous, heavy operation.',
        },
        {
          title: 'How do you secure these networks?',
          description: 'Distinct networks are allocated for specific purposes, embracing the principle of \'separation of concerns\'. These networks grant internet access only, restricting local access unless explicitly required. All equipment receives monthly security and stability updates and supports the ‘best practise’ WPA3 security standard.',
        },
        {
          title: 'Can your networks be customized to integrate existing systems?',
          description: 'In the preliminary consultation phase, our network experts understand any existing equipment and configuration to ensure seamless integration.',
        },
        {
          title: 'How do you keep costs this low for the end-user?',
          description: 'wifiOne leverages cutting-edge enterprise equipment with cloud management; this means no additional on-premises management equipment. Equipment is highly integrated, reducing the number of devices, licensing and management burden.',
        },
      ],
    }
  },
  mounted() {
    const jquery = window.$
    jQuery('.iq-accordion .iq-accordion-block .accordion-details').hide()
    // jQuery('.iq-accordion .iq-accordion-block:first').addClass('accordion-active').children().slideDown('slow')
    jQuery('.iq-accordion .iq-accordion-block').on('click', function () {
      jQuery('.iq-accordion .iq-accordion-block').not(this).removeClass('accordion-active').children('div.accordion-details ').slideUp('slow');
      jQuery(this).toggleClass('accordion-active').children('div.accordion-details ').slideToggle('slow');
    })
  }
}
</script>
<style scoped>
.accordion-title:before {
  background: transparent !important;
  color: #3F81D1 !important;
  box-shadow: none !important;
  font-size: 30px;
}

.accordion-description {
  color: #343E59;
  font-size: 18px;
  font-style: normal;
  font-weight: 400;
}
</style>
