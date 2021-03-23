<template>
  <div>
    <swiper>
      <swiper-item v-for="item in banners">
        <template #default>
          <a :href="item.link">
            <img :src="item.image" alt="">
          </a>
        </template>
      </swiper-item>
    </swiper>
  </div>
</template>

<script>
  
  import {Swiper, SwiperItem} from 'components/common/swiper'

  export default {
    name: 'HomeSwiper',
    components: {
      Swiper,
      SwiperItem
    },
    props: {
      banners: {
        type: Array,
        default() {
          return []
        }
      }
    }
    
  }
</script>

<style scope>
  
</style>