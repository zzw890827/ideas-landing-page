<template>
  <div data-spy="scroll" data-offset="80">
    <Loader/>
    <HeaderStyle1 :logo-img="logo" :nav-item-list="navItems" :styled-logo="styleLogo"/>
    <nuxt/>
  </div>
</template>
<script>
import logoImg from '../assets/images/logo.png'

export default {
  name: 'LandingPage1',
  head() {
    return {
      bodyAttrs: {
        'data-spy': 'scroll',
        'data-offset': '80'
      }
    }
  },
  data() {
    return {
      styleLogo: false,
      logo: logoImg,
      navItems: [
        {
          href: '#iq-home',
          title: 'ホーム',
          active: true,
          // children: true,
          // child: [
          //   {
          //     href: '/landing-page-1',
          //     title: 'Landing page 1'
          //   },
            // {
            //   href: '/landing-page-2',
            //   title: 'Landing page 2'
            // },
            // {
            //   href: '/landing-page-3',
            //   title: 'Landing page 3'
            // },
            // {
            //   href: '/landing-page-4',
            //   title: 'Landing page 4'
            // },
            // {
            //   href: '/landing-page-5',
            //   title: 'Landing page 5'
            // },
            // {
            //   href: '/landing-page-6',
            //   title: 'Landing page 6'
            // }
          //]
        },
        {href: '#how-it-works', title: '会社概要'},
        {href: '#software-features', title: 'サービス'},
        /* { href: '#great-screenshots', title: 'Screenshots' }, */
        {href: '#pricing', title: '採用情報'},
        {href: '#team', title: '組織'},
        // {href: '#blog', title: 'ブログ'},
        {href: '#contact-us', title: '連絡'}
      ]
    }
  },
  mounted() {
  }
}
</script>
<style>
@import url('../assets/css/color/style.css');

.wow {
  visibility: hidden;
}

@keyframes fadeInUp {
  0% {
    opacity: 0;
    -webkit-transform: translate3d(0, 30%, 0);
    -ms-transform: translate3d(0, 30%, 0);
    transform: translate3d(0, 30%, 0);
  }
  100% {
    opacity: 1;
    -webkit-transform: none;
    -ms-transform: none;
    transform: none;
  }
}

.fadeInUp {
  animation-name: fadeInUp;
  animation-timing-function: ease-out;
}
</style>
