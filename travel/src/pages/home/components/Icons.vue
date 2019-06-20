<template>
  <div class="icons">
    <swiper>
      <swiper-slide v-for="(page,index) of pages" :key="index">
        <div class="icon" v-for="item of page" :key="item.id">
          <div class="icon-img">
            <img class="icon-img-content" :src="item.imgUrl">
          </div>
          <p class="icon-desc">{{item.desc}}</p>
        </div>
      </swiper-slide>
    </swiper>
  </div>
</template>

<script>
export default {
  name: 'HomeIcons',
  data () {
    return {
      iconList: [
        {
          id: 'ooo1',
          imgUrl:
            'http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png',
          desc: '景点门票'
        },
        {
          id: 'ooo2',
          imgUrl:
            'http://img1.qunarzz.com/piao/fusion/1804/5a/13ceb38dcf262f02.png',
          desc: '一日游'
        },
        {
          id: 'ooo3',
          imgUrl:
            'http://img1.qunarzz.com/piao/fusion/1804/ff/fdf170ee89594b02.png',
          desc: '成都必游'
        },
        {
          id: 'ooo4',
          imgUrl:
            'http://img1.qunarzz.com/piao/fusion/1803/e3/67df61427c8e1302.png',
          desc: '川剧变脸'
        },
        {
          id: 'ooo5',
          imgUrl:
            'http://img1.qunarzz.com/piao/fusion/1803/b6/aae239efe3496602.png',
          desc: '成都火锅'
        },
        {
          id: 'ooo6',
          imgUrl:
            'http://img1.qunarzz.com/piao/fusion/1803/b8/c5dcdb58deec2402.png',
          desc: '碧峰峡'
        },
        {
          id: 'ooo7',
          imgUrl:
            'http://img1.qunarzz.com/piao/fusion/1803/95/8246f27355943202.png',
          desc: '国色天香'
        },
        {
          id: 'ooo8',
          imgUrl:
            'http://img1.qunarzz.com/piao/fusion/1803/54/35899492b1302802.png',
          desc: '熊猫基地'
        },
        {
          id: 'ooo9',
          imgUrl:
            'http://img1.qunarzz.com/piao/fusion/1804/5a/13ceb38dcf262f02.png',
          desc: '光明顶'
        }
      ]
    }
  },
  computed: {
    pages () {
      const pages = []
      this.iconList.forEach((item, index) => {
        const page = Math.floor(index / 8)
        if (!pages[page]) {
          pages[page] = []
        }
        pages[page].push(item)
      })
      return pages
    }
  }
}
</script>

<style lang = "stylus" scoped>
@import '~styles/varibles.styl';
@import '~styles/mixins.styl';

.icons >>> .swiper-container {
  height: 0;
  padding-bottom: 50%;
  /* background-color: red; */
  /* 占位 */
}

.icon {
  width: 25%;
  height: 0;
  float: left;
  padding-bottom: 25%;
  overflow: hidden;
  position: relative;
}

.icon-img {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0.44rem;
  padding: 0.1rem;
  box-sizing: border-box;
}

.icon-img-content {
  display: block;
  margin: 0 auto;
  height: 100%;
}

.icon-desc {
  position: absolute;
  left: 0;
  right: 0;
  bottom: 0;
  height: 0.44rem;
  line-height: 0.44rem;
  text-align: center;
  color: $darkTextColor;
  ellipsis()
}
</style>
