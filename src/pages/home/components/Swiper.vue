<template>
  <div class="warpper">
    <swiper :options="swiperOption">
      <swiper-slide v-for="(item, i) in swiperList" :key="i">
        <img class="swiper-img" :src="item.imgUrl" alt="" >
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
        pagination: '.swiper-pagination',
        loop: true
      },
      swiperList: [
        {
          id: '0001',
          imgUrl: 'https://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20193/c5e84c198ca6a3e8b7e9946144ebefb5.jpg_750x200_43eebad0.jpg'
        },
        {
          id: '0002',
          imgUrl: 'https://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20193/942d87cc1576c333c77dc1f86af145cd.jpg_750x200_d25bf3eb.jpg'
        },
        {
          id: '0003',
          imgUrl: 'https://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20193/d7bbc21db442366a882e04ddc984669a.jpg_750x200_85e640d9.jpg'
        },
        {
          id: '0004',
          imgUrl: 'https://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20193/278a88f18f1523eec8c52f650522be68.jpg_750x200_bc365244.jpg'
        }
      ]
    }
  }
}
</script>
<style lang="stylus" scpoed>
  .swiper-pagination-bullet-active
    background: #fff
  .warpper
    overflow: hidden
    width: 100%
    height: 0
    padding-bottom: 31.25%
  .swiper-img
    width: 100%
</style>
