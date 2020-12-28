<template>
  <q-btn
    @click="$emit('locationClicked')"
    class="footerbtn"
    flat
    unelevated
    ><slot></slot></q-btn
  >
</template>

<script>
export default {
  name: 'btnFooter'
}
</script>

<style lang="scss" scoped>
.footerbtn {
  height: 52px;
}
</style>