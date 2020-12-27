<template>
      <q-drawer
      side="right"
      v-model="drawer"
      show-if-above
      :mini="miniState"
      @mouseover="miniState = false"
      @mouseout="miniState = true"
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
          <h4>cards will be there</h4>
        </div>
      </q-scroll-area>
    </q-drawer>
</template>

<script>
export default {
  name: 'rightDrawer',
  data() {
    return {
      drawer: false,
      miniState: true
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
</style>