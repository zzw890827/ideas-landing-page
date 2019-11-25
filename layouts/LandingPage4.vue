<template>
  <div data-spy="scroll" data-offset="80">
    <Loader />
    <HeaderStyle2 :logo-img="logo" :nav-item-list="navItems" :styled-logo="true" class-name="header-white">
      <!--      <a href="#" class="button bt-black pull-right" slot="navContent">Download</a>-->
    </HeaderStyle2>
    <nuxt />
  </div>
</template>

<script>
import logoImg from '../assets/images/logo-footer.png'
export default {
  name: 'LandingPage4',
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
        { href: '#software-features', title: 'Service' },
        /* { href: '#great-screenshots', title: 'Screenshots' }, */
        { href: '#great-features', title: 'Features' },
        { href: '#blog', title: 'Blog' },
        { href: '#contact', title: 'Contact' }
      ]
    }
  },
  mounted () {
  }
}
</script>

<style>
    @import url('../assets/css/color/style.css');
</style>
