<template>
  <div id="home">
    首页
    <!-- <nav-bar class="home-nav">
      <div slot="center">
        购物街
      </div>
    </nav-bar> -->
    <!-- <tab-control class="tab-control"
                  :titles="['流行','新款','精选']"
                  @tabClick="tabClick"
                  ref = "tabControl1"
                  v-show="isTabFixed"
                  ></tab-control>
    <scroll class="content" ref="scroll" 
            :probe-type="3" 
            @scroll="contentScroll"
            :pull-up-load="true" 
            @pullingUp = "loadMore">
      <home-swiper :banners='banners'
                    @swiperImageLoad="swiperImageLoad"/>
      <recommend-view :recommends='recommends'></recommend-view>
      <feature-view></feature-view>
      <tab-control :titles="['流行','新款','精选']"
                  @tabClick="tabClick"
                  ref = "tabControl2"
                  ></tab-control>
      <good-list :goods="showGoods"></good-list>

    </scroll>
    <!--当我们需要监听一个组件的原生事件时，必须给对应的事件加上.native修饰符-->
    <!-- <back-top @click.native="backTop" v-show="isShowBackTop"></back-top>  -->

  </div>
</template>

<script>

// import HomeSwiper from './ChildComps/HomeSwiper';
// import RecommendView from './ChildComps/RecommendView';
// import FeatureView from './ChildComps/FeatureView';

// import NavBar from 'components/common/navbar/NavBar';
// import TabControl from 'components/content/tabControl/TabControl';
// import GoodList from 'components/content/goods/GoodsList';
// import Scroll from 'components/common/scroll/Scroll';


// import {
//   getHomeMultidata,
//   getHomeGoods
//   } from 'network/home';
// import {debounce} from 'common/utils';
// import {itemListenerMixin, backTopMixin} from 'common/mixin';
// import {BACK_POSITION} from 'common/const';

export default {
  name: 'Home',
  
 }
</script>

<style  scoped>
#home{
  /* padding-top: 44px; */
  height: 100vh;
  position: relative;
}
.home-nav{
  background-color: var(--color-tint);
  color: #fff;
/* 
  position: fixed;
  left: 0;
  right: 0;
  top: 0;
  z-index: 9; */
}
.tab-control{
  position: relative;
  
  z-index: 9;
}
.content{
    overflow: hidden;

    position: absolute;
    top: 44px;
    bottom: 49px;
    left: 0;
    right: 0;
}
</style> 