<template>
  <!-- wrapper: read comment in styles section -->
  <div class="wrapper">
    <q-card class="choose-location" style="width:1000px">
      <q-btn
        class="choose-location__button bg-primary"
        text-color="white"
        dense
        outline
        flat
        v-close-popup
        ><q-icon name="close" color="white" />
      </q-btn>
      <q-card-section>
        <span class="choose-location__title text-accent">Veldu stað</span>
      </q-card-section>
      <q-card-section class="q-pt-none">
        <btnLocationBig
          class="q-ma-xs"
          v-for="(location, idx) in locations"
          :key="idx"
        >
          {{ location }}
        </btnLocationBig>
      </q-card-section>
    </q-card>
  </div>
</template>

<script>
import btnLocationBig from 'src/tokyodark/components/buttons/btnLocationBig'
export default {
  name: 'chooseLocation',
  components: { btnLocationBig },
  data() {
    return {
      locations: [
        'Glæsibær',
        'Krónan Flatahraun',
        'Krónan Lindir',
        'Nýbýlavegur'
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
// wrapper needed to provide space for close button which is hanging partly outside modal window
.wrapper {
  padding: 20px;
  display: flex;
  box-shadow: none;
  max-width: 940px;
}
.choose-location {
  display: flex;
  flex-direction: column;
  align-items: center;

  &__title {
    font-family: 'Anton';
    font-size: 36px;
    text-transform: capitalize;
    align-self: center;
  }

  &__button {
    border-radius: 50%;
    width: 40px;
    height: 40px;
    position: absolute;
    right: -20px;
    top: -20px;
  }
}
</style>
