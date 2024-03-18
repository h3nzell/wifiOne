<template>
  <section class="aboutus-two-service pb-0">
    <div class="container">
      <div class="row">
        <div class="col-lg-4 col-md-6 mb-5" v-for="(list,index) in items" :key="index">
          <CardStyle1>
            <div slot="cardMedia">
              <img :src="list.src" alt="fancy-list">
            </div>
            <div slot="cardTitle">
              <h5 class="mb-2">{{ list.title }}</h5>
            </div>
            <div slot="cardBody">
              <p>{{ list.description }}</p>
            </div>
            <div slot="cardInfo">
              <p class=" font-weight-bold mt-4">{{ list.info }}</p>
            </div>
            <div slot="cardLink">
              <div class="blog-button w-100 d-flex justify-content-end">
                <a :href="list.link" class="button blue-btn button-icon text-left">Learn More</a>
              </div>
            </div>
          </CardStyle1>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
import CardStyle1 from '../themes/Card/CardStyle1'
export default {
  name: 'Services',
  components: { CardStyle1 },
  data() {
    return{
      items : [
        {
          title: 'Managed WiFi and Network ',
          description: 'Reliable & high-performance WiFi is crucial for your office\'s online communication, collaboration and cloud applications. Seeking a scalable solution with comprehensive coverage and support with proactive monitoring to prevent disruptions?\n' + 'We provide a seamless setup, responsive provider, and transparent pricing. This will boost your productivity and efficiency.',
          src: require('../../assets/images/home/services/01.png'),
          link: '/managed-wifi'
        },
        {
          title: 'Event WiFi Solutions',
          description: 'We offer flexible event WiFi solutions for seamless attendee connectivity: online registration, networking, social media, and mobile payments. Scalable for various sizes and locations with guaranteed coverage and bandwidth options.\n' +
            'Reliable WiFi allows instant connectivity for all your attendees for a positive experience. Hassle-free setup is a game-changer for event organizers wanting a simple solution.',
          src: require('../../assets/images/home/services/02.png'),
          link: '/event-wifi'
        },
        {
          title: 'Managed Cameras and Access Systems',
          description: 'Choose Managed Cameras and Access Systems service for enhanced security and peace of mind. This includes remote real-time monitoring whilst keeping around a month of history. You will get high-definition cameras with wide coverage, smart alerts and support, accessible anywhere from your laptop or smartphone.\n' +
            'We ensure a reliable and secure service based on your business needs.',
          src: require('../../assets/images/home/services/03.png'),
          link: '/managed-cameras'
        },
        {
          title: 'Managed Multi-Zone Music Speakers',
          description: 'With Managed Multi-Zone Music Speakers service you can create an immersive audio experience for your cafe or restaurant. This will elevate customer retention, boost sales and contribute to a positive brand image.\n' +
            'Key features are high-fidelity sound, intuitive control, diverse music sources and remote management from your laptop or smartphone.',
          src: require('../../assets/images/home/services/04.png'),
          link: '/managed-music-system'
        },
        {
          title: 'Site Power Monitoring',
          description: 'Site Power Monitoring enables you to gain valuable insights into energy consumption and identify cost savings. This will help us optimize usage, reduce our carbon footprint, and improve overall efficiency.\n' +
            'Our service will empower you to make strides in energy monitoring, as well as to minimize your environmental impact, and contribute to the sustainability of your business.',
          src: require('../../assets/images/home/services/05.png'),
          link: '/site-power-monitoring'
        },
        {
          title: 'Managed media wall/signage',
          description: 'Managed Media Wall/Signage introduces radical new options for brand awareness and marketing. You can visually-engaging signage to attract the target audience to your products and branding.\n' +
            'Multiple advertising campaigns can be scheduled, all managed remotely for instant updates and diagnostics to ensure uninterrupted, seamless brand awareness and marketing.',
          src: require('../../assets/images/home/services/06.png'),
          link: '/managed-media-wall'
        }
      ]
    }
  }
}
</script>
