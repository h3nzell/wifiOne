<template>
  <section>
    <div class="container">
      <div class="row">
        <div class="col-lg-4 col-sm-12 sidebar-service-left">
          <CardStyle5 :card-menu="menu_item" />
        </div>
        <div class="col-lg-8 col-sm-12 pt-5 pt-lg-0">
          <h1 class="service-title">Why do you need this service?</h1>
          <p>Your current WiFi network is unreliable causing event disruptions and frustrating attendees. Limited data and insights into attendee behavior, difficulty scaling WiFi to accommodate large crowds.</p>
          <h1 class="service-title">our solution</h1>
          <p>Enjoy seamless and consistent WiFi coverage throughout our entire office space, with minimal to no downtime or dead zones. Protect your sensitive data and company network from cyber threats. We’ll be the provider who proactively monitors your network health and resolves potential issues before they impact you.</p>
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
          class: 'nav-link current-menu-item',
          href: 'event-wifi'
        },
        {
          title: 'Managed Cameras',
          class: 'nav-link',
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
