<template>
  <a :href="link" class="font-bold py-2 px-3 text-white rounded-lg hover:bg-secondary">{{ text }}</a>
</template>

<script>
export default {
  name: 'NavTopItem',
  props: {
    text: {
      required: true,
      type: String
    },
    link: {
      required: true,
      type: String
    }
  }
}
</script>

<style>

</style>
