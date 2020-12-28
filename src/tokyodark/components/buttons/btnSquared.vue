<template>
        <q-btn
        class="btn-squared bg-primary"
        text-color="white"
        dense
        outline
        flat
        v-close-popup
        ><slot/>
      </q-btn>
</template>

<script>
export default {
  name: 'btnSquared'

}
</script>

<style lang='scss' scoped>
.btn-squared {
  width: 24px;
  height: 25px;
  line-height: 25px;
  
}

</style>