<template>
  <div id="stock-information">
    <div class="flex">
      <div
        v-on:click="thisTab"
        data-tab="0"
        class="tab w-1/5 mx-2 py-2 border-2 border-light-grey"
      >
        Quote & Chart
      </div>
      <div
        v-on:click="thisTab"
        data-tab="1"
        class="tab w-1/5 mx-2 py-2 border-2 border-light-grey"
      >
        Tab 2
      </div>
      <div
        v-on:click="thisTab"
        data-tab="2"
        class="tab w-1/5 mx-2 py-2 border-2 border-light-grey"
      >
        Tab 3
      </div>
      <div
        v-on:click="thisTab"
        data-tab="3"
        class="tab w-1/5 mx-2 py-2 border-2 border-light-grey"
      >
        Tab 4
      </div>
      <div
        v-on:click="thisTab"
        data-tab="4"
        class="tab w-1/5 mx-2 py-2 border-2 border-light-grey"
      >
        Tab 5
      </div>
    </div>
    <div class="tab-content">
      <div id="tab-0" v-if="currentTab == 0">
        <h1>tab 1</h1>
      </div>
      <div id="tab-1" v-if="currentTab == 1">
        <h1>tab 2</h1>
      </div>
      <div id="tab-2" v-if="currentTab == 2">
        <h1>tab 3</h1>
      </div>
      <div id="tab-3" v-if="currentTab == 3">
        <h1>tab 4</h1>
      </div>
      <div id="tab-4" v-if="currentTab == 4">
        <h1>tab 5</h1>
      </div>
    </div>
  </div>
</template>
<style lang="scss">
.tab {
  @apply flex items-center justify-center rounded;
}
</style>
<script>
export default {
  data() {
    return {
      currentTab: 0
    };
  },
  methods: {
    thisTab(e) {
      console.log(e.target.dataset.tab);
      this.currentTab = e.target.dataset.tab;
    }
  }
};
</script>
