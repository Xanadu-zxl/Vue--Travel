<template>
  <div class="wrapper">
    <swiper :options="swiperOption">
      <swiper-slide v-for="item of swiperList" :key="item.id">
        <img class="swiper-img" :src="item.imgUrl" alt="轮播图">
      </swiper-slide>
      <div class="swiper-pagination" slot="pagination"></div>
    </swiper>
  </div>
</template>

<script>
export default {
  name: 'HomeSwiper',
  data () {
    return {
      swiperOption: {
        pagination: '.swiper-pagination', // 导航条
        loop: true// 循环
      },
      swiperList: [
        {
          id: '0001',
          imgUrl:
            'https://f-flightfe-portalcp.qunarzz.com/f_flightfe_portal_f_flightfe_portal/2019/1547807426824_26157347.jpg'
        },
        {
          id: '0002',
          imgUrl:
            'http://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20196/7f52250d5a61b170f4b568510b194c20.jpg_750x200_de78880a.jpg'
        },
        {
          id: '0003',
          imgUrl:
            'http://img1.qunarzz.com/piao/fusion/1807/5e/cfee2e9e2f357202.jpg_750x200_b0308a43.jpg'
        }
      ]
    }
  }
}
</script>

<style lang = "stylus" scoped>
.wrapper >>> .swiper-pagination-bullet-active {
  background: #fff;
}

.wrapper {
  width: 100%;
  height: 0;
  overflow: hidden;
  padding-bottom: 31.25%;
  background: #eee;
}

.swiper-img {
  width: 100%;
  height: 31.25%;
}
</style>
