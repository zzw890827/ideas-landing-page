<template>
  <section id="pricing" class="overview-block-ptb grey-bg iq-price-table">
    <div class="container">
      <div class="row">
        <div class="col-sm-12">
          <div class="heading-title">
            <h3 class="title iq-tw-7">採用情報</h3>
            <p>仲間になって、夢を叶えよう！</p>
          </div>
        </div>
      </div>
      <div class="row">
        <div class="col-md-4 col-lg-4">
          <div class="iq-pricing text-center">
            <PricingCardStyle2>
              <div slot="cardHeader">
                <span class="text-uppercase iq-tw-4 iq-font-white">ソフトエンジニア</span>
              </div>
              <ul slot="cardList">
                <li>XXXX</li>
                <li>XXXX</li>
                <li>XXXX</li>
                <li>XXXX</li>
              </ul>
              <div slot="cardFooter">
                <a class="button" href="javascript:void(0)">Entry</a>
              </div>
            </PricingCardStyle2>
          </div>
        </div>
        <div class="col-md-4 col-lg-4">
          <PricingCardStyle2>
            <div slot="cardHeader">
              <span class="text-uppercase iq-tw-4 iq-font-white">システムエンジニア</span>
            </div>
            <ul slot="cardList">
              <li>XXXX</li>
              <li>XXXX</li>
              <li>XXXX</li>
              <li>XXXX</li>
            </ul>
            <div slot="cardFooter">
              <a class="button" href="javascript:void(0)">Entry</a>
            </div>
          </PricingCardStyle2>
        </div>
        <div class="col-md-4 col-lg-4 r4-mt-30">
          <PricingCardStyle2>
            <div slot="cardHeader">
              <span class="text-uppercase iq-tw-4 iq-font-white">プロジェクトマネージャー</span>
            </div>
            <ul slot="cardList">
              <li>XXXX</li>
              <li>XXXX</li>
              <li>XXXX</li>
              <li>XXXX</li>
            </ul>
            <div slot="cardFooter">
              <a class="button" href="javascript:void(0)">Entry</a>
            </div>
          </PricingCardStyle2>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  name: 'Pricing'
}
</script>
