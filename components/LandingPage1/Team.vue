<template>
  <section id="team" class="overview-block-ptb white-bg">
    <div class="container">
      <div class="row">
        <div class="col-sm-12">
          <div class="heading-title">
            <h3 class="title iq-tw-7">
              組織
            </h3>
          </div>
        </div>
      </div>
      <div class="row">
        <div class="col-sm-12 col-lg-3 col-md-6" v-for="(item,index) of list" :key="index">
          <CardStyle8>
            <img slot="cardMedia" v-rjs="3" :src="item.image" class="img-fluid center-block" alt="#">
            <div slot="cardHeader">
              <h5 class="iq-font-black iq-tw-7">
                {{ item.title }}
              </h5>
              <span class="team-post">{{ item.subtitle }}</span>
            </div>
            <div slot="cardOverlay">
              <ul>
                <li><a href="javascript:void(0)"><i class="fab fa-twitter"/></a></li>
                <li><a href="javascript:void(0)"><i class="fab fa-facebook"/></a></li>
                <li><a href="javascript:void(0)"><i class="fab fa-google"/></a></li>
                <li><a href="javascript:void(0)"><i class="fab fa-github"/></a></li>
              </ul>
            </div>
          </CardStyle8>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  name: 'Team',
  data() {
    return {
      list: [
        {
          title: '景 斌',
          subtitle: '代表取締役社長',
          image: require('../../assets/images/team/01.png')
        },
        {
          title: 'XXXX',
          subtitle: '経営執行役',
          image: require('../../assets/images/team/02.png')
        },
        {
          title: 'XXXX',
          subtitle: '執行役（非常勤）',
          image: require('../../assets/images/team/03.png')
        },
        {
          title: 'XXX',
          subtitle: '顧問',
          image: require('../../assets/images/team/04.png')
        }
      ]
    }
  }
}
</script>
