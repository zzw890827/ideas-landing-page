<template>
  <div data-spy="scroll" data-offset="80">
    <Loader />
    <HeaderStyle1 :logo-img="logo" :nav-item-list="navItems" :styled-logo="styleLogo">
      <a slot="navContent" href="#" class="button bt-black pull-right">Download</a>
    </HeaderStyle1>
    <nuxt />
  </div>
</template>

<script>
import logoImg from '../assets/images/logo.png'
export default {
  name: 'LandingPage5',
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
        { href: '#about-us', title: 'About' },
        /* { href: '#great-screenshots', title: 'Screenshots' }, */
        { href: '#feature', title: 'Feature' },
        { href: '#how-it-works', title: 'Service' },
        { href: '#our-pricing', title: 'Pricing' },
        { href: '#testimonial', title: 'Testimonial' },
        { href: '#get-in-tech', title: 'Contact' }
      ]
    }
  }
}
</script>

<style>
    @import url('../assets/css/color/style.css');
</style>
