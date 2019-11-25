<template>
  <section class="overview-block-ptb grey-bg iq-specialities">
    <div class="container">
      <div class="row">
        <div class="col-sm-12">
          <div class="heading-title">
            <h3 class="title iq-tw-7">
              グルメオーダーリングサービス
            </h3>
            <p>扫码点餐一句话概括XXXXXXXXX</p>
          </div>
        </div>
      </div>
      <div class="row">
        <div v-for="item of list" :key="item.id" class="col-sm-12 col-lg-3 col-md-6 iq-mb-30">
          <CardStyle6>
            <i slot="cardMedia" aria-hidden="true" :class="item.icon"></i>
            <div slot="cardBody">
              <h5 class="iq-tw-7 iq-pt-20 iq-pb-10">
                {{ item.title }}
              </h5>
              <p v-for="(e, index) of item.description" :key="index">{{e}}</p>
            </div>
          </CardStyle6>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  name: 'Specialites',
  data () {
    return {
      list: [
        {
          id: '0001',
          icon: 'ion-qr-scanner',
          title: 'QRコードで料理のスマホ注文',
          description: ['人員不足対策', '大幅コストダウン']
        },
        {
          id: '0002',
          icon: 'ion-social-chrome',
          title: 'ノーアプリインストール',
          description: ['ブラウザあれば使用可能', 'お客様負担なし'],
        },
        {
          id: '0003',
          icon: 'ion-arrow-graph-up-right',
          title: 'データ分析機能標準搭載',
          description: ['店舗データ見える化', '管理をスマートに'],
        },
        {
          id: '0004',
          icon: 'ion-ios-heart-outline',
          title: '7/24/365安心サポート',
          description: ['いつでもサポート', '安心、安全'],
        },
      ]
    }
  }
}
</script>
