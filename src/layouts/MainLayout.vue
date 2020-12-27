<template>
  <q-layout view="hHr lpr fFr" class="app-layout">
    <!-- <q-header class="bg-primary text-white" height-hint="98">
      <q-tabs align="left" class="toptab">
        <q-route-tab to="/page1" label="Page One" />
        <q-route-tab to="/page2" label="Page Two" />
        <q-route-tab to="/page3" label="Page Three" />
      </q-tabs>
    </q-header> -->
    <main-header />
    <right-drawer/>
    <q-page-container>
      <router-view />
    </q-page-container>
    <main-footer></main-footer>
  </q-layout>
</template>

<style lang="scss">
.toptab {
  background-color: rgba(0, 0, 0, 0);
}

.app-layout {
  background-image: url("~assets/Main Image@1x.png");
  background-size: cover;
  background-repeat: no-repeat;
  background-position-x: center;
  background-position-y: center;
}
</style>

<script>
import mainHeader from "src/tokyodark/layouts/mainHeader";
import rightDrawer from 'src/tokyodark/layouts/rightDrawer';
import mainFooter from 'src/tokyodark/layouts/mainFooter';
export default {
  name: "MainLayout",
  components: { mainHeader, rightDrawer, mainFooter },

};
</script>
