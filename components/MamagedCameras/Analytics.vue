<template>
  <section>
    <div class="container">
      <div class="row ">
        <div class="col-lg-4 col-sm-12 sidebar-service-left ">
          <CardStyle5 :card-menu="menu_item" />
        </div>
        <div class="col-lg-8 col-sm-12 pt-5 pt-lg-0">
          <h1 class="service-title">Why do you need this service?</h1>
          <p>You've experienced the shortcomings of inadequate security solutions in the past, leading to costly incidents and disruptions. Today, you seek a trusted partner who can deliver a robust and smoothly integrated system that enhances security, improves operational efficiency, and provides peace of mind.</p>
          <h1 class="service-title">our solution</h1>
          <p>WifiOne Managed Cameras and Access Systems provide comprehensive security solutions with high-definition cameras, advanced access control, and 24/7 monitoring. These features simplify access management and improve operational efficiency. Real-time video feeds and alerts offer real-time insights into activity and enable quick response to incidents.</p>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  name: 'Analytics',
  data () {
    return {
      menu_item: [
        {
          title: 'Managed WiFi',
          class: 'nav-link ',
          href: 'managed-wifi'
        },
        {
          title: 'Event WiFi Solutions',
          class: 'nav-link',
          href: 'event-wifi'
        },
        {
          title: 'Managed Cameras',
          class: 'nav-link current-menu-item',
          href: 'managed-cameras'
        },
        {
          title: 'Managed Music Systems',
          class: 'nav-link',
          href: 'managed-music-system'
        },
        {
          title: 'Site Power Monitoring',
          class: 'nav-link',
          href: 'site-power-monitoring'
        },
        {
          title: 'Managed media wall',
          class: 'nav-link',
          href: 'managed-media-wall'
        },
      ]
    }
  }
}
</script>
<style>
.service-title {
  color: #3F81D1;
  font-size: 30px;
  font-style: normal;
  font-weight: 600;
  line-height: normal;
  text-transform: uppercase;
}
</style>
