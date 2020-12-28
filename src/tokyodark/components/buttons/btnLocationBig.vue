<template>
  <q-btn class="btn-location-big bg-secondary" text-color="accent" unelevated>
    <div class="btn-location-big__content">
      <small-twisted-logo size="43px" class="btn-location-big__logo" />
      <slot></slot>
    </div>
  </q-btn>
</template>

<script>
import smallTwistedLogo from 'src/tokyodark/components/logos/smallTwistedLogo'
export default {
  name: 'btnLocationBig',
  components: { smallTwistedLogo },
  data: () => ({})
}
</script>

<style lang="scss" scoped>
.btn-location-big {
  width: 207px;
  height: 202px;
  text-transform: capitalize;
  font-family: BarlowCondensed;
  font-size: 20px;

  &__content {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  &__logo {
    margin-bottom: 6px;
  }
}
</style>
