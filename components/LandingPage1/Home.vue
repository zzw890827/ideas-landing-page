<template>
  <ParallaxStyle1 ids="iq-home" :bg-image="bgImage"
                  class-names="iq-banner overview-block-pt iq-bg-over iq-over-blue-90 iq-parallax">
    <div class="container-fluid">
      <div class="banner-text">
        <div class="row">
          <div class="col-lg-6">
            <h1 class="text-uppercase iq-font-white iq-tw-3">
              お客様に100％の <b class="iq-tw-7">満足</b>
            </h1>
            <p class="iq-font-white iq-pt-15 iq-mb-40">
              ソフトウェアを開発・提供する会社にとって、お客様に100％の「満足」をいただくことが、究極の目的であり、
              会社の安定・発展の基であると考えております。今後、アイデアズグループという安定した事業基盤を背景に人員増強、
              売上・利益拡大を図り、近い将来の株式公開を目指しています。
            </p>
          </div>
          <div class="col-lg-6">
            <img class="banner-img" :src="require('../../assets/images/banner/01.png')" alt="">
          </div>
        </div>
      </div>
    </div>
    <div class="banner-objects">
      <span class="banner-objects-01" data-bottom="transform:translatey(50px)" data-top="transform:translatey(-50px);">
        <img :src="require('../../assets/images/drive/03.png')" alt="drive02">
      </span>
      <span class="banner-objects-02 iq-fadebounce">
        <span class="iq-round"/>
      </span>
      <span class="banner-objects-03 iq-fadebounce">
        <span class="iq-round"/>
      </span>
    </div>
  </ParallaxStyle1>
</template>
<script>
export default {
  name: 'Home',
  data() {
    return {
      bgImage: require('../../assets/images/bg/01.jpg')
    }
  }
}
</script>
