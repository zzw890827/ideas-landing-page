<template>
  <div data-spy="scroll" data-offset="80">
    <Loader />
    <HeaderStyle1 :logo-img="logo" :nav-item-list="navItems" :styled-logo="styleLogo" class="header-one">
<!--
      <a slot="navContent" href="#" class="button bt-black pull-right">Download</a>
-->
      <TopbarStyle1 slot="topBar">
        <ul slot="leftLinks">
          <li><a href="#"><i class="fa fa-phone iq-mr-10" aria-hidden="true" /><span class="iq-font-white">+1234567890</span></a></li>
        </ul>
        <ul slot="rightLinks">
          <li><a href="#"><i class="fab fa-facebook-f" /></a></li>
          <li><a href="#"><i class="fab fa-twitter" /></a></li>
          <li><a href="#"><i class="fab fa-pinterest" /></a></li>
          <li><a href="#"><i class="fab fa-google-plus-g" /></a></li>
        </ul>
      </TopbarStyle1>
    </HeaderStyle1>
    <nuxt />
  </div>
</template>

<script>
import logoImg from '../assets/images/logo-footer.png'
import TopbarStyle1 from '../components/sofbox/Partials/Topbar/TopbarStyle1'

export default {
  name: 'LandingPage6',
  components: { TopbarStyle1 },
  head () {
    return {
      bodyAttrs: {
        'data-spy': 'scroll',
        'data-offset': '80'
      }
    }
  },

  data () {
    return {
      styleLogo: false,
      logo: logoImg,
      navItems: [
        { href: '#iq-home',
          title: 'Home',
          active: true,
          children: true,
          child: [
            {
              href: '/landing-page-1',
              title: 'Landing page 1'
            },
            {
              href: '/landing-page-2',
              title: 'Landing page 2'
            },
            {
              href: '/landing-page-3',
              title: 'Landing page 3'
            },
            {
              href: '/landing-page-4',
              title: 'Landing page 4'
            },
            {
              href: '/landing-page-5',
              title: 'Landing page 5'
            },
            {
              href: '/landing-page-6',
              title: 'Landing page 6'
            }
          ]
        },
        { href: '#how-it-works', title: 'About' },
        /* { href: '#great-screenshots', title: 'Screenshots' }, */
        { href: '#software-features', title: 'Service' },
        { href: '#team', title: 'Team' },
        { href: '#pricing', title: 'Pricing' },
        { href: '#blog', title: 'Blog' },
        { href: '#contact', title: 'Contact' }
      ]
    }
  }
}
</script>

<style>
    @import url('../assets/css/color/style.css');

</style>
