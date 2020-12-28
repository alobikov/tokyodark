<template>
  <div class="landing-promo">
    <div class="landing-promo__title bg-accent">
      <span>
        check out our new lunch offers
      </span>
    </div>
    <div class="landing-promo__details">
      <span>
        Select from Sushi, Mixed and hot offers. Available from Monday through
        Friday from 11:30 - 14:00.
      </span>
    </div>
    <btnMeira />
  </div>
</template>

<script>
import btnMeira from 'src/tokyodark/components/buttons/btnMeira'
export default {
  name: 'landingPromo',
  components: { btnMeira }
}
</script>

<style lang="scss" scoped>
.landing-promo {
  width: 543px;
  display: flex;
  flex-direction: column;
  position: absolute;
  top: 35%;
  left: 105px;
  &__title {
    font-family: 'Anton';
    font-size: 40px;
    color: white;
    text-transform: capitalize;
    padding: 10px 20px 2px 15px;
    border-radius: 2px;
    margin-bottom: 31px;
  }
  &__details {
    font-family: 'BarlowCondensed';
    font-size: 20px;
    color: white;
    margin-bottom: 26px;
  }
}
</style>
