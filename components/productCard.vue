<template>
  <!-- <div class="border-gray-400 h-96 shadow-lg border-solid p-6 bg-white rounded-xl text-center mx-5 my-4">
    <img style="width:40%" class="mx-auto" src="https://newannapurnatoursandtravels.com/deep/hospitania/website/assets/img/product/product-2.png">

    <div class="rounded-md  p-5">
      <h2 class="text-xl">
        Panadol
      </h2>
    </div>
  </div> -->
  <div class="product-card">
    <div
      class="
    product-card-content absolute top-0 left-0 w-full h-full"
    >
      <img class="mx-auto" style="width:33%" src="https://newannapurnatoursandtravels.com/deep/hospitania/website/assets/img/product/product-2.png">
      <div class="flex flex-col space-y-4 p-5 justify-center">
        <h2 class="text-lg font-bold">
          Sarang Organic Kalonji 100 gm Pack
        </h2>
        <h3>120$</h3>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'ProductCard'
}
</script>
<style scoped>
.product-card::after{
  content: '';
  display: block;
  position: relative;
  padding-top:120% ;
margin-left: 20px;
margin-right: 20px;
}

/* .product-image{
  height: 200px;
} */
</style>
