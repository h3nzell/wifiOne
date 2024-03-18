<template>
  <section>
    <div class="container">
      <div class="row">
        <div class="col-lg-4 col-sm-12 sidebar-service-left">
          <CardStyle5 :card-menu="menu_item" />
        </div>
        <div class="col-lg-8 col-sm-12 pt-5 pt-lg-0">
          <h1 class="service-title">Why do you need this service?</h1>
          <p>You don’t know when power failure has occurred, leaving your office and staff out of operation. Worse, any electromagnetic (EM) doors will be unlocked and camera systems offline, putting your site at risk of theft or intrusion, particularly after office hours.</p>
          <h1 class="service-title">our solution</h1>
          <p>wifiOne Site Power Monitoring provides you instant notification when power failure occurs. <br> This allows you to dispatch your facilities personnel to turn the tripped circuit breaker back on, restoring operations, network and security.</p>
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
          class: 'nav-link current-menu-item',
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
