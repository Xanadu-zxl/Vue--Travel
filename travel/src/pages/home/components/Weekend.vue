<template>
  <div>
    <div class="title">周末去哪儿</div>
    <ul>
      <li class="item border-bottom" v-for="item of weekendList" :key="item.id">
        <div class="item-img-wrapper">
          <img class="item-img" :src="item.imgUrl">
        </div>
        <div class="item-info">
          <p class="item-title">{{item.title}}</p>
          <p class="item-desc">{{item.desc}}</p>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HomeWeekend',
  data () {
    return {
      weekendList: [
        {
          id: '0001',
          imgUrl:
            'http://img1.qunarzz.com/sight/p64/201211/04/9173ff9f33e97f3193835fbb.jpg_640x276_0a0474d5.jpg',
          title: '成都杜甫草堂',
          desc: '草堂有水，有桥，有庭院'
        },
        {
          id: '0002',
          imgUrl:
            'http://img1.qunarzz.com/sight/p0/1505/b0/b0132e78efa00572.water.jpg_640x276_b87d3bb4.jpg',
          title: '青城山',
          desc: '青城山有白素贞？？'
        },
        {
          id: '0003',
          imgUrl:
            'http://img1.qunarzz.com/sight/p0/201309/24/977fea7b3c5cd758c8d65eac.jpg_640x276_915af8e3.jpg',
          title: '成都大雄猫繁育研究基地',
          desc: '在这里与各种大小熊猫亲密接触&拍照合影'
        },
        {
          id: '0004',
          imgUrl:
            'http://img1.qunarzz.com/sight/p0/201407/03/a584374ee80b738e2600d6bcaf1299e3.jpg_640x276_ba327700.jpg',
          title: '都江堰',
          desc: '世界水利工程的鼻祖'
        }
      ]
    }
  }
}
</script>

<style lang="stylus" scoped>
@import '~styles/mixins.styl';

.title {
  line-height: 0.8rem;
  background: #eee;
  text-indent: 0.2rem;
}

.item-img-wrapper {
  overflow: hidden;
  height: 0;
  padding-bottom: 37.09%;
}

.item-img {
  width: 100%;
}

.item-info {
  padding: 0.1rem;
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
</style>
