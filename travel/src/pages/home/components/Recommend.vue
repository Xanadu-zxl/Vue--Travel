<template>
  <div>
    <div class="title">热销推荐</div>
    <ul>
      <li class="item border-bottom" v-for="item of recommendList" :key="item.id">
        <img class="item-img" :src="item.imgUrl"/>
        <div class="item-info">
          <p class="item-title">{{item.title}}</p>
          <p class="item-desc">{{item.desc}}</p>
          <button class="item-button">查看详情</button>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HomeRecommend',
  data () {
    return {
      recommendList: [
        {
          id: '0001',
          imgUrl:
            'http://img1.qunarzz.com/sight/p0/1905/32/32ad7003179269d2a3.img.jpg_200x200_aee761e4.jpg',
          title: '谭鸭血老火锅（太古里直营店）',
          desc: '好吃的板丶真滴偶偶偶偶'
        },
        {
          id: '0002',
          imgUrl:
            'http://img1.qunarzz.com/sight/p0/1612/1d/1d9a740c1f9e0efaa3.img.jpg_200x200_63285bd9.jpg',
          title: '成都海昌极地海洋公园',
          desc: '好玩的板丶真滴偶偶偶偶'
        },
        {
          id: '0003',
          imgUrl:
            'http://img1.qunarzz.com/sight/p0/1704/a5/a59677101e07d38a3.img.jpg_200x200_6064e939.jpg',
          title: '那是飞一样的感觉，国色天乡',
          desc: '嗨皮的板丶真滴偶偶偶偶'
        },
        {
          id: '0004',
          imgUrl:
            'http://img1.qunarzz.com/sight/p0/201407/03/a584374ee80b738e2600d6bcaf1299e3.jpg_200x200_c26fb243.jpg',
          title: '都江堰',
          desc: '良辰美景，值得一来'
        }
      ]
    }
  }
}
</script>

<style lang="stylus" scoped>
@import '~styles/mixins.styl';

.title {
  margin-top: 0.2rem;
  line-height: 0.8rem;
  background: #eee;
  text-indent: 0.2rem;
}

.item {
  overflow: hidden;
  display: flex;
  height: 1.9rem;
}

.item-img {
  width: 1.7rem;
  height: 1.7rem;
  padding: 0.1rem;
}

.item-info {
  flex: 1;
  padding: 0.1rem;
  min-width: 0;
}

.item-title {
  line-height: 0.54rem;
  font-size: 0.32rem;
  ellipsis();
}

.item-desc {
  line-height: 0.4rem;
  color: #ccc;
  ellipsis();
}

.item-button {
  line-height: 0.44rem;
  margin-top: 0.16rem;
  background: #ff9300;
  padding: 0 0.2rem;
  border-radius: 0.06rem;
  color: #fff;
}
</style>
