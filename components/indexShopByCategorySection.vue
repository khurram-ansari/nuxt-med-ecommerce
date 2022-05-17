<template>
  <div class="px-8">
    <h2 class="my-8 text-3xl font-bold">
      Shop by category
    </h2>
    <swiper
      :slides-per-view="5"
      :autoplay="true"
      :loop="false"
    >
      <swiper-slide
        v-for="(cat,i) in categories"
        :key="i"
      >
        <category-card :category="cat" />
      </swiper-slide>
    </swiper>
  </div>
</template>

<script>
import { Navigation, Pagination } from 'swiper'

import { SwiperCore, Swiper, SwiperSlide } from 'swiper-vue2'

// Import Swiper styles
import 'swiper/swiper-bundle.css'
import categoryCard from './categoryCard.vue'
SwiperCore.use([Navigation, Pagination])
export default {
  name: 'IndexShopByCategorySection',
  components: {
    categoryCard,
    Swiper,
    SwiperSlide
  },
  data () {
    return {
      categories: [
        {
          name: 'Darjeeling Teas',
          image: 'https://newannapurnatoursandtravels.com/deep/hospitania/website/assets/img/category/category-2.png'
        },
        {
          name: 'Covid Masks',
          image: 'https://newannapurnatoursandtravels.com/deep/hospitania/website/assets/img/category/category-5.png'
        },
        {
          name: 'Whey Protein',
          image: 'https://newannapurnatoursandtravels.com/deep/hospitania/website/assets/img/category/category-3.png'
        },
        {
          name: 'Nutrition',
          image: 'https://newannapurnatoursandtravels.com/deep/hospitania/website/assets/img/category/category-4.png'
        },
        {
          name: 'Hand Sanitizer',
          image: 'https://newannapurnatoursandtravels.com/deep/hospitania/website/assets/img/category/category-8.png'
        }
      ]
    }
  }

}
</script>

<style>

</style>
