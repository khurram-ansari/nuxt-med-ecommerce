<template>
  <div class="px-8">
    <h2 class="my-8 text-3xl font-bold">
      Featured products
    </h2>
    <swiper
      :breakpoints="swiperBreakPoints"
      :slides-per-view="5"
      :autoplay="true"
      :loop="false"
    >
      <swiper-slide
        v-for="(n,i) in 10"
        :key="i"
      >
        <product-card />
      </swiper-slide>
    </swiper>
  </div>
</template>

<script>
import { Navigation, Pagination } from 'swiper'

import { SwiperCore, Swiper, SwiperSlide } from 'swiper-vue2'

// Import Swiper styles
import 'swiper/swiper-bundle.css'
import ProductCard from './productCard.vue'
SwiperCore.use([Navigation, Pagination])
export default {
  name: 'IndexFeaturedProducts',
  components: {
    Swiper,
    SwiperSlide,
    ProductCard
  },
  data () {
    return {
      swiperBreakPoints: {
        320: {
          slidesPerView: 2
        },
        // when window width is >= 480px
        480: {
          slidesPerView: 3
        },
        // when window width is >= 640px
        640: {
          slidesPerView: 4
        },
        820: {
          slidesPerView: 5
        }
      }
    }
  }
}
</script>
