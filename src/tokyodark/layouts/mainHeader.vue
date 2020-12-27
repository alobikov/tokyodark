<template>
  <q-header class="transparent">
    <q-toolbar class='header__toolbar'>
      <small-twisted-logo class="header__logo"/>
      <span>MATSEÐILL</span>
      <span>TILBOÐ</span>
      <span>VEISLUBAKKAR</span>
      <span>ENG</span>

      <q-toolbar-title></q-toolbar-title>
       <btnMittTokyo />
      <btnPanta class="q-ml-sm" />
    </q-toolbar>
  </q-header>
</template>

<script>
import btnPanta from "src/tokyodark/components/buttons/btnPanta";
import btnMittTokyo from "src/tokyodark/components/buttons/btnMittTokyo";
import smallTwistedLogo from "src/tokyodark/components/logos/smallTwistedLogo";
export default {
  name: "mainHeader",
  components: { btnPanta, btnMittTokyo, smallTwistedLogo }
};
</script>

<style lang="scss" scoped>
.header__toolbar {
  padding: 20px;
}
.header__title {
  width: 40%;
  flex: 0 1 100px;
}
.header__wrapper {
  height: 100%;
  width: 100%;
  padding: 0 20px;
}
.header__logo {
  margin-right: 15px;
}
span {
  font-family: MainFont;
  font-style: normal;
  font-weight: 800;
  font-size: 15px;
  // line-height: 18px;
  letter-spacing: 0.25em;
  padding: 0 15px 0 15px;
}
</style>
