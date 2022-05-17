<template>
  <div>
    <section>
      <index-hero-section />
    </section>
    <section>
      <index-shop-by-category-section />
    </section>
    <section>
      <index-featured-products />
    </section>
  </div>
</template>

<script>
import indexHeroSection from '../components/indexHeroSection.vue'
import IndexShopByCategorySection from '~/components/indexShopByCategorySection.vue'
import IndexFeaturedProducts from '~/components/indexFeaturedProducts.vue'
export default {
  name: 'IndexPage',
  components: { indexHeroSection, IndexShopByCategorySection, IndexFeaturedProducts },
  layout: 'mainLayout'
}
</script>
