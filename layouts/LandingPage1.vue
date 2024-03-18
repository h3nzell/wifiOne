<template>
    <div>
      <HeaderStyle1 :logo-img="logo" :nav-item-list="navItems" class-name="style-one" :styled-logo="styleLogo" />
      <nuxt />
      <ScrollTop />
    </div>
</template>
<script>
import {menu, services, pages, landing1About, ourCases, blog, contacts} from '../config/constant.js'
import logoImg from '../assets/images/logo_1.svg'
export default {
  name: 'LandingPage1',
  data () {
    return {
      styleLogo: true,
      logo: logoImg,
      navItems: [
        { href: '/landing-page',
          title: 'Home',
          active: true,
          children: false,
          child: menu,
          classname: 'menu'
        },
        { href: '/about', title: 'About Us', children: false, child: landing1About, classname: ' ' },
        { href: '/services', title: 'Services', children: true, child: services, classname: ' ' },
        { href: '/customers', title: 'Customers', active: true, children: false, child: pages, classname: ' '  },
        { href: '/contact-us', title: 'Contact Us', children: false, child: contacts, classname: ' ' }
      ]
    }
  },
  mounted () {
  }
}
</script>
<style>
  @import url('../assets/css/style.css');
  @import url('../assets/css/responsive.css');
</style>
