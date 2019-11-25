<template>
  <div>
    <Home />
    <div class="main-content">
      <About />
      <Specialities />
      <Counter />
      <Testimonial />
      <Pricing />
      <Team />
      <footer>
        <Contact />
        <FooterStyle3>
          <p slot="address">東京都港区芝浦2丁目14番8号 第2ﾃｰﾜｲﾋﾞﾙ7F</p>
          <p slot="phone">03-5439-4371
            <br>Mon-Fri 8:00am - 8:00pm
            <br>
          </p>
          <p slot="mail">support@sofbox.com
            <br>24 X 7 online support
            <br>
          </p>
          <ul slot="links">
            <li><a href="javascript:void(0)"><i class="fab fa-twitter"></i></a></li>
            <li><a href="javascript:void(0)"><i class="fab fa-facebook"></i></a></li>
            <li><a href="javascript:void(0)"><i class="fab fa-google"></i></a></li>
            <li><a href="javascript:void(0)"><i class="fab fa-github"></i></a></li>
          </ul>
        </FooterStyle3>
      </footer>
    </div>
    <ColorCustomizer />
    <ScrollTop />
  </div>
</template>

<script>
import Home from '../../components/LandingPage1/Home'
import About from '../../components/LandingPage1/About'
import Specialities from '../../components/LandingPage1/Specialities'
import Counter from '../../components/LandingPage1/Counter'
import Testimonial from '../../components/LandingPage1/Testimonial'
import Pricing from '../../components/LandingPage1/Pricing'
import Team from '../../components/LandingPage1/Team'
import Contact from '../../components/LandingPage1/Contact'
import { sofbox } from '../../assets/app/app'

export default {
  layout: 'LandingPage1',
  components: {
    Home,
    About,
    Specialities,
    Counter,
    Testimonial,
    Pricing,
    Team,
    Contact
  },
  mounted () {
    setTimeout(function () {
      sofbox.index()
      // sofbox.magnific()
    }, 1000)
  }
}
</script>
