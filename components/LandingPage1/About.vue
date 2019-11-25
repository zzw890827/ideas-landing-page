<template>
  <div>
    <section id="how-it-works" class="overview-block-ptb it-works">
      <div class="container">
        <div class="row">
          <div class="col-sm-12">
            <div class="heading-title">
              <h3 class="title iq-tw-7">株式会社アイデアズ</h3>
              <p>企业口号XXXXXX</p>
            </div>
          </div>
        </div>
        <div class="row">
          <div class="col-md-12 col-lg-4">
            <CardStyle5 step="1">
              <img slot="cardMedia" src="../../assets/images/services/icon1.png" class="img-fluid" alt="#">
              <div slot="cardBody">
                <h5 class="iq-tw-7 iq-mt-25 iq-mb-15">
                  企業理念
                </h5>
                <p>xxx xxxx xxx xx xxxxx xxx xxxxx bxxx xxxxs. xxx xxxx xxxx. xxx x x x x xx</p>
              </div>
            </CardStyle5>
          </div>
          <div class="col-md-12 col-lg-4 r-mt-30">
            <CardStyle5 step="2">
              <img slot="cardMedia" src="../../assets/images/services/icon2.png" class="img-fluid" alt="#">
              <div slot="cardBody">
                <h5 class="iq-tw-7 iq-mt-25 iq-mb-15">
                  アワーミッション
                </h5>
                <p>xxx xxxx xxx xx xxxxx xxx xxxxx bxxx xxxxs. xxx xxxx xxxx. xxx xxxx xxxx xxxx xxxx xxx</p>
              </div>
            </CardStyle5>
          </div>
          <div class="col-md-12 col-lg-4 r-mt-30">
            <CardStyle5 step="3">
              <img slot="cardMedia" src="../../assets/images/services/icon3.png" class="img-fluid" alt="#">
              <div slot="cardBody">
                <h5 class="iq-tw-7 iq-mt-25 iq-mb-15">
                  ゴール
                </h5>
                <p>xxx xxxx xxx xx xxxxx xxx xxxxx bxxx xxxxs. xxx xxxx xxxx. xxx xxxx xxxx xxxx xxxx xxx</p>
              </div>
            </CardStyle5>
          </div>
        </div>
      </div>
    </section>
    <SectionStyle1>
      <div slot="cardBody" class="col-lg-6">
        <div class="heading-title left text-left">
          <h3 class="iq-tw-7 iq-mb-25 title">
            会社案内
          </h3>
        </div>
        <p>商号：株式会社アイデアズ</p>
        <p>略称：IDEAS Co.,Ltd.</p>
        <p>資本金：2,800万円(日本本社)</p>
        <p>創立：2001年3月27日</p>
        <p>従業員数：50名(日本本社)</p>
        <p>加盟団体：一般社団法人 日本ソフトウェアー産業協会 (NSA)</p>
      </div>
      <div slot="cardMedia" class="col-lg-6 align-self-center">
        <img class="iq-works-img pull-right img-fluid" src="../../assets/images/drive/01.png" alt="drive01">
      </div>
    </SectionStyle1>
    <SectionStyle2 id="software-features" :small="small">
      <div slot="cardMedia" class="iq-software-demo">
        <img class="img-fluid" src="../../assets/images/drive/05.png" alt="drive05">
      </div>
      <div slot="cardBody" class="col-lg-6 offset-lg-6">
        <div class="heading-title left text-left">
          <h3 class="iq-tw-7 iq-mb-25 title">
            業務紹介
          </h3>
        </div>
        <p>
          お客様に満足して頂くために、アイデアズグループは、社員一人一人のアイデアを出し、
          長年培った豊富な経験・知識と最新の技術を融合させた高度技術化集団を目指し、
          社員一同がソフトウェアの開発・各種サービスの提供にあたり、常に社会貢献を念頭におき取り組んでおります。</p>
        <ul class="iq-mt-40 iq-list">
          <li class="iq-tw-6 iq-mb-15">
            <i class="ion-android-done-all iq-mr-10 iq-font-blue iq-font-30"></i>
            <span class="iq-font-black">
              １．グルメオーダーリングサービス
            </span>
          </li>
          <li class="iq-tw-6 iq-mb-15">
            <i class="ion-android-done-all iq-mr-10 iq-font-blue iq-font-30"></i>
            <span class="iq-font-black">
              ２．ハンディターミナルシステム
            </span>
          </li>
          <li class="iq-tw-6 iq-mb-15">
            <i class="ion-android-done-all iq-mr-10 iq-font-blue iq-font-30"></i>
            <span class="iq-font-black">
              ３．免税書類作成ハンディシステム
            </span>
          </li>
          <li class="iq-tw-6 iq-mb-15">
            <i class="ion-android-done-all iq-mr-10 iq-font-blue iq-font-30"></i>
            <span class="iq-font-black">
              ４．モバイル決済サービス
            </span>
          </li>
        </ul>
      </div>
    </SectionStyle2>
  </div>
</template>
<script>
export default {
  name: 'About',
  data() {
    return {
      small: true
    }
  }
}
</script>
