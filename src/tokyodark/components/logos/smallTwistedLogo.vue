<template>
  <q-img
    calss="absolute-center"
    :width="size"
    :height="size"
    src="~assets/logoTwistedSmall.svg"
  />
</template>

<script>
export default {
  name: 'smallTwistedLogo',
  props: ['size']
}
</script>

<style lang="scss" scoped>
.scoped-image {
  margin: 21px;
}
</style>
