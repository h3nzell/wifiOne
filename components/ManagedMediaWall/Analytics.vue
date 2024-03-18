<template>
  <section>
    <div class="container">
      <div class="row">
        <div class="col-lg-4 col-sm-12 sidebar-service-left">
          <CardStyle5 :card-menu="menu_item" />
        </div>
        <div class="col-lg-8 col-sm-12 pt-5 pt-lg-0">
          <h1 class="service-title">Why do you need this service?</h1>
          <p>Your current signage is unreliable and requires constant maintenance. It lacks the flexibility and modern features to effectively communicate with our audience.</p>
          <h1 class="service-title">our solution</h1>
          <p>Managed Media Wall/Signage provides a scalable and reliable solution to manage your digital signage needs. This frees you from technical headaches and allows you to focus on creating engaging content.</p>
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
          class: 'nav-link ',
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
          class: 'nav-link current-menu-item',
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
