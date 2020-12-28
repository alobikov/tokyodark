<template>
      <q-drawer
      side="right"
      v-model="drawer"
      show-if-above
      :mini="miniState"
      @mouseover="miniState = false"
      @mouseout="miniState = false"
      :mini-width="80"
      :width="450"
      :breakpoint="500"
      bordered
      content-class="white col"
    >
      <q-scroll-area class="fit">
        <div class="row">
          <q-list class="drawer__container" padding>
            <q-img
              class="drawer__imageTop"
              width="80px"
              src="~assets/waves.png"
            ></q-img>
            <q-img
              class="drawer__imageCenter"
              width="50px"
              src="~assets/tokyo-logo-vertical.svg"
            ></q-img>
            <q-img
              class="drawer__imageBottom"
              width="80px"
              src="~assets/waves.png"
            ></q-img>
          </q-list>
          <q-separator vertical inset color="lightgrey"></q-separator>
          <div class="right-column ">
          <itemCard/>
          <q-separator inset></q-separator>
            <div class="drawer-totals q-px-md q-mt-lg">
              <span class='text-accent q-mr-xs'>Samtals</span>
              <span class='text-primary'>9.990 kr.</span>
            </div>
          <basket-controls></basket-controls>
          </div>
        </div>
      </q-scroll-area>
    </q-drawer>
</template>

<script>
import basketControls from "src/tokyodark/components/cards/basketControls"
import itemCard from "src/tokyodark/components/cards/itemCard"
export default {
  name: 'rightDrawer',
  components: {basketControls, itemCard},
  data() {
    return {
      drawer: false,
      miniState: false
    };
  }
}
</script>

<style lang='scss' scoped>
.drawer__container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  height: 100vh;
}
.drawer__imageCenter {
  margin: 18px 0 18px 15px;
}
.drawer__imageTop {
  flex: 1 1;
  opacity: 0;
}
.drawer__imageBottom {
  flex: 1 1;
}
.right-column {
  flex: 1;
  height: 600px;
}
.drawer-totals {
  span {
    font-family: 'BarlowCondensed';
    font-size: 20px;
  }

}
</style>