<template>
  <nav class="flex bg-primary-900 p-5 ">
    <nav-top-logo />
    <div class="flex mx-auto space-x-4 items-center">
      <nav-top-item v-for="item in menuItems" :key="item.link" :text="item.text" :link="item.link" />
    </div>
  </nav>
</template>

<script>
import navTopItem from './navTopItem.vue'
import NavTopLogo from './navTopLogo.vue'
export default {
  name: 'NavTop',
  components: { navTopItem, NavTopLogo },
  data () {
    return {
      menuItems: [
        {
          text: 'Home',
          link: '/dashboard'
        },
        {
          text: 'About',
          link: '/about'
        }
      ]
    }
  }
}
</script>

<style>

</style>
