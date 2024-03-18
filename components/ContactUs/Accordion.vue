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
  data () {
    return {
      items: [
        {
          title: 'What differentiates you from the competitors?',
          description: 'wifiOne prioritizes reliability and performance for cost-sensitive markets by employing top-tier enterprise equipment. This ensures optimal connectivity, meeting high standards without compromising affordability, delivering a seamless experience for our clients.',
        },
        {
          title: 'How do you ensure fair sharing of a single internet connection among multiple networks?',
          description: 'wifiOne implements a tiered Quality of Service approach, allocating bandwidth to prioritize mission-critical network services. This guarantees smooth and lag-free real-time conferencing and VoIP/Skype/Teams calling.',
        },
        {
          title: 'How does wifiOne safeguard my business or event from cyber threats?',
          description: 'wifiOne keeps each network isolated from one another; devices on each network are isolated from each other by default also. Finally, infrastructure devices receive monthly security and bugfix updates to prevent intrusion.',
        },
        {
          title: 'Can you integrate with existing networks?',
          description: 'You can choose between a “no changes” approach on your existing network, where wifiOne’s equipment will be put on a separate upstream or downstream network, or “maximum quality” approach for the highest performance, security and reliability where we change out the infrastructure equipment for the managed service, keeping all the other devices connected.',
        },
      ],
    }
  },
  mounted () {
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
<style  scoped>
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
