<template>
  <div>
    <swiper
      :slides-per-view="1"
      :autoplay="true"
      :loop="false"
      @swiper="onSwiper"
      @slideChange="onSlideChange"
    >
      <swiper-slide
        v-for="(n,i) in slides"
        :key="i"
        class="test"
      >
        <img
          :src="n"
          class="w-full object-cover"
        >
      </swiper-slide>
    </swiper>
  </div>
</template>

<script>
import { Navigation, Pagination } from 'swiper'

import { SwiperCore, Swiper, SwiperSlide } from 'swiper-vue2'

// Import Swiper styles
import 'swiper/swiper-bundle.css'
SwiperCore.use([Navigation, Pagination])
export default {
  name: 'IndexHeroSection',
  components: {
    Swiper,
    SwiperSlide
  },
  data () {
    return {
      slides: [require('~/assets/banner1.png'), require('~/assets/banner2.png')]
    }
  },
  methods: {
    getImageUrl (imageId) {
      return `https://picsum.photos/1280/450/?image=${imageId}`
    },
    onSwiper (swiper) {
      console.log(swiper)
    },
    onSlideChange () {
      console.log('slide change')
    }
  }
}
</script>

<style>

</style>
