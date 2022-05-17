<template>
  <div>
    <navbar-top />
    <div>
      <nuxt />
    </div>
  </div>
</template>

<script>
import NavbarTop from '../components/navTop.vue'
export default {
  name: 'MainLayout',
  components: { NavbarTop }
}
</script>

<style>

</style>
