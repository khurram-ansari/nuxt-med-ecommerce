<template>
  <div class="border-gray-400 bg-primary-50 border-solid p-6 rounded-xl text-center mx-5 my-4">
    <div class="category-image my-4">
      <img class="mx-auto w-3/4" :src="category.image">
    </div>

    <div class="rounded-md category-card-details p-5">
      <h2 class="text-xl">
        {{ category.name }}
      </h2>
    </div>
  </div>
  <!-- <div class="mx-5 category-card bg-primary-50 text-center my-4 min-h-48 overflow-hidden rounded-md">
    <img class="w-3/5 mx-auto -mb-6" src="https://newannapurnatoursandtravels.com/deep/hospitania/website/assets/img/category/category-8.png">
    <div class="rounded-md category-card-details bg-primary-900 p-8">
      <h2 class="text-xl font-bold text-white">
        Vitamins
      </h2>
    </div>
  </div> -->
  <!-- <div class="rounded-full min-h-48 mx-5 my-4 text-center bg-gradient-to-b from-primary-50 to-primary-50">
    <img class="w-3/5 mx-auto " src="https://newannapurnatoursandtravels.com/deep/hospitania/website/assets/img/category/category-8.png">
    <h2 class="text-xl font-bold ">
      Vitamins
    </h2>
  </div> -->
</template>

<script>
export default {
  name: 'CategoryCard',
  props: {
    category: {
      required: true,
      type: Object
    }
  }

}
</script>

<style scoped>
.category-card:hover .category-card-details {
    transition: all 0.5s;
background:theme('colors.secondary');
}
.category-image{
  height: 180px;
}

</style>
