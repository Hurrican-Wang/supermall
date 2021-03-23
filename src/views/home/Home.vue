<template>
  <div>
    <nav-bar class="home-nav">
      <template #center>
        购物街
      </template>
    </nav-bar>
    <home-swiper :banners="banners"></home-swiper>
  </div>
</template>

<script>
  import NavBar from 'components/common/navbar/NavBar'
  import HomeSwiper from './homeswiper/HomeSwiper'
  import {getHomeMultidata} from 'network/home'
  
  
  export default {
    name: 'Home',
    components: {
      NavBar,
      HomeSwiper
    },
    data() {
      return {
        banners: [],
        recommends: []
      }
    },
    created() {
      getHomeMultidata().then(res => {
        this.banners = res.data.banner.list;
        this.recommends = res.data.recommend.list;
        // console.log(res.data);
      })
    }
  }
</script>

<style scope>
  .home-nav {
    background-color: var(--color-tint);
    color: #fff;
  }
</style>