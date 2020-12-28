<template>
  <q-footer bordered class="bg-dark text-white">
    <q-toolbar class="toolbar-xpadding">
      <q-toolbar-title class="row justify-start items-center no-wrap">
        <div class="footer-right-icons row no-wrap">
          <q-img
            class="margin-right-12"
            width="19px"
            height="19px"
            src="~assets/cameraIcn.svg"
          />
          <q-img
            class="marign-right-15"
            width="19px"
            height="19px"
            src="~assets/facebookIcn.svg"
          />
        </div>
        <div class="row justify-between items-center full-width">
          <div class="row items-center ">
            <btnStadirnir @locationClicked="$emit('locationClicked')" />
            <span>UM OKKUR</span>
            <span>HAFÐU SAMBAND</span>
          </div>
          <div class="row">
            <span class="line-height-23">NÁÐU Í APPIÐ</span>
            <q-img
              class="margin-right-12"
              width="19px"
              height="23px"
              src="~assets/androidIcn.svg"
            />
            <q-img
              class="marign-right-15"
              width="19px"
              height="23px"
              src="~assets/iosIcn.svg"
            />
          </div>
        </div>
      </q-toolbar-title>
    </q-toolbar>
  </q-footer>
</template>

<script>
import btnStadirnir from 'src/tokyodark/components/buttons/btnStadirnir'
export default {
  name: 'mainFooter',
  components: { btnStadirnir }
}
</script>

<style lang="scss" scoped>
.toolbar-xpadding {
  padding: 0 20px;
}
span {
  font-family: MainFont;
  font-style: normal;
  font-weight: 800;
  font-size: 12px;
  letter-spacing: 0.25em;
  padding: 0 15px 0 15px;
  line-height: 19px;
}
.margin-right-15 {
  margin-right: 15px;
}
.margin-right-12 {
  margin-right: 12px;
}
.line-height-23 {
  line-height: 23px;
}
</style>
