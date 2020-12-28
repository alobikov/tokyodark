<template>
  <q-btn
    @click="$emit('breytaClicked')"
    class="btn-breyta"
    flat
    unelevated
    >BREYTA</q-btn
  >
</template>

<script>
export default {
  name: 'btnBreyta'
}
</script>

<style lang="scss" scoped>
.btn-breyta {
  height: 25px;
  font-size: 12px;
  font-weight: 800;
  color: $accent;
  letter-spacing: 0.25em;

}
</style>