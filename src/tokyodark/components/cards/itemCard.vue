<template>
  <q-card flat square>
    <q-card-section horizontal>
    <q-card-section class="item-card__leftrow">
      <q-img ratio="1" src="~assets/dish.png"></q-img>
    </q-card-section>
    <q-card-section class="item-card__rightrow">
      <q-list dense>
        <q-item dense class="item-card__title">Kjúklinga Katsu poké</q-item>
        <q-item dense class="item-card__description">Poke bowl base selection</q-item>
        <q-item dense class="item-card__type">Sushi hrisgrjón</q-item>
        <div class="item-card__controls q-pl-md q-py-sm">
          <div class="item-card__controls-noflex"><btn-squared><q-icon class="absolute-center" size="16px" name="remove" color="white" /></btn-squared></div>
          <div class='item-card__amount item-card__controls-noflex'>2</div>
          <div class="item-card__controls-noflex"><btn-squared><q-icon class="absolute-center" size="16px" name="add" color="white" /></btn-squared></div>
          <div class="item-card__controls-noflex"><btn-breyta/></div>
        </div>
        <q-item dense class="item-card__price">4.995 kr.</q-item>
      </q-list>

    </q-card-section>
    </q-card-section>
  </q-card>
</template>

<script>
import btnBreyta from 'src/tokyodark/components/buttons/btnBreyta'
import btnSquared from 'src/tokyodark/components/buttons/btnSquared'
export default {
  name: 'itemCard',
  components: {btnBreyta, btnSquared}

}
</script>

<style lang="scss" scoped>
.item-card {
  &__leftrow {
    flex: 1 0;
    padding-right: 0;
  }
  &__rightrow {
    flex: 3 1;
    padding-left: 0;
  }
  &__title {
    font-family: "BarlowCondensed";
    font-size: 20px;
    font-weight: 700;
    color: $accent;
  }
  &__description {
    font-family: 'Roboto';
    font-size: 18px;
    color: $midgrey;
    margin-left: 0;
  }
  &__type {
    font-family: "Roboto";
    font-weight: 500;
    font-size: 18px;
    margin-left: 0px;
  }
  &__price {
    font-family: "BarlowCondensed";
    font-size: 20px;
    font-weight: 700;
    margin-left: 0;
    color: $primary;
  }
  &__amount {
    font-family: 'Anton';
    font-size: 18px;
    padding: 0 12px;
  }
  &__controls {
    display: flex;
    justify-content: flex-start;
    align-items: center;
    &-noflex {
      flex: 0;
    }
  }
}
</style>