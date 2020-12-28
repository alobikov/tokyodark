<template>
  <q-btn
    @click="$emit('locationClicked')"
    class="footerbtn appbtn-size-md"
    flat
    unelevated
    >STAÐIRNIR</q-btn
  >
</template>

<script>
export default {
  name: 'btnStadirnir'
}
</script>

<style lang="scss" scoped></style>
