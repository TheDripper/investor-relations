<template>
  <div id="stock-information">
    <div class="max-w-6xl mx-auto mt-12">
      <h1>Stock Information</h1>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
        tempor incididunt ut labore et dolore magna aliqua.
      </p>
    </div>

    <div class="max-w-6xl mx-auto mt-8">
      <div class="flex tabs">
        <div
          v-on:click="thisTab"
          :class="{ active: currentTab == 0 }"
          data-tab="0"
          class="tab w-1/5  py-2 border border-light-grey"
        >
          <p>Quote & Chart</p>
        </div>
        <div
          v-on:click="thisTab"
          :class="{ active: currentTab == 1 }"
          data-tab="1"
          class="tab w-1/5  py-2 border border-light-grey"
        >
          <p>Tab 2</p>
        </div>
        <div
          v-on:click="thisTab"
          :class="{ active: currentTab == 2 }"
          data-tab="2"
          class="tab w-1/5  py-2 border border-light-grey"
        >
          <p>Tab 3</p>
        </div>
        <div
          v-on:click="thisTab"
          :class="{ active: currentTab == 3 }"
          data-tab="3"
          class="tab w-1/5  py-2 border border-light-grey"
        >
          <p>Tab 4</p>
        </div>
        <div
          v-on:click="thisTab"
          :class="{ active: currentTab == 4 }"
          data-tab="4"
          class="tab w-1/5  py-2 border border-light-grey"
        >
          <p>Tab 5</p>
        </div>
      </div>
      <div class="tab-content py-24 px-12 border border-grey">
        <div id="tab-0" v-if="currentTab == 0">
          <div class="flex w-full">
            <div style="flex:33%;" class="p-6">
              <img src="/stock-price.png" />
            </div>
            <div class="flex justify-center" style="flex:66%;">
              <div style="flex:50%;">
                <div
                  class="flex w-full items-center justify-between p-6 border-t border-light-grey"
                >
                  <label>Label</label>
                  <p>Value</p>
                </div>
                <div
                  class="flex w-full items-center justify-between p-6 border-t border-light-grey"
                >
                  <label>Label</label>
                  <p>Value</p>
                </div>
                <div
                  class="flex w-full items-center justify-between p-6 border-t border-light-grey"
                >
                  <label>Label</label>
                  <p>Value</p>
                </div>
                <div
                  class="flex w-full items-center justify-between p-6 border-t border-light-grey"
                >
                  <label>Label</label>
                  <p>Value</p>
                </div>
              </div>
              <div style="flex:50%;">
                <div
                  class="flex w-full items-center justify-between p-6 border-t border-light-grey"
                >
                  <label>Label</label>
                  <p>Value</p>
                </div>
                <div
                  class="flex w-full items-center justify-between p-6 border-t border-light-grey"
                >
                  <label>Label</label>
                  <p>Value</p>
                </div>
                <div
                  class="flex w-full items-center justify-between p-6 border-t border-light-grey"
                >
                  <label>Label</label>
                  <p>Value</p>
                </div>
                <div
                  class="flex w-full items-center justify-between p-6 border-t border-light-grey"
                >
                  <label>Label</label>
                  <p>Value</p>
                </div>
              </div>
            </div>
          </div>
          <div class="max-w-6xl mx-auto mt-8">
            <h2 class="mb-8">Stock Performance</h2>
            <img class="" src="/stock.png" />
          </div>

          <div class="max-w-6xl mx-auto mt-8">
            <h2 class="mb-8">Historical Dividend</h2>
            <table>
              <thead>
                <tr>
                  <th>Label</th>
                  <th>Label</th>
                  <th>Label</th>
                  <th>Label</th>
                  <th>Label</th>
                </tr>
              </thead>
              <tbody>
                <tr>
                  <td>Value</td>
                  <td>Value</td>
                  <td>Value</td>
                  <td>Value</td>
                  <td>Value</td>
                </tr>
                <tr>
                  <td>Value</td>
                  <td>Value</td>
                  <td>Value</td>
                  <td>Value</td>
                  <td>Value</td>
                </tr>
                <tr>
                  <td>Value</td>
                  <td>Value</td>
                  <td>Value</td>
                  <td>Value</td>
                  <td>Value</td>
                </tr>
                <tr>
                  <td>Value</td>
                  <td>Value</td>
                  <td>Value</td>
                  <td>Value</td>
                  <td>Value</td>
                </tr>
                <tr>
                  <td>Value</td>
                  <td>Value</td>
                  <td>Value</td>
                  <td>Value</td>
                  <td>Value</td>
                </tr>
              </tbody>
            </table>
            <p class="text-xs text-light-grey mt-12 px-16">
              Nulla felis dolor, tincidunt quis felis vel, fringilla consequat
              ligula. Donec congue et est sit amet consectetur. Morbi aliquet
              sollicitudin arcu, sit amet mattis purus eleifend eget. Sed
              convallis ligula ligula, et varius enim elementum quis. Etiam
              congue iaculis mi, non feugiat metus viverra eu. Quisque egestas
              mauris eu erat luctus tristique. Sed aliquet tellus id tortor
              molestie, rhoncus semper enim aliquam. Etiam pretium, turpis nec
              tincidunt viverra, erat lacus pellentesque lectus, quis euismod
              nulla nisi vel nibh. Cras sed posuere diam, eget lacinia lacus.
              Fusce diam eros, dignissim id imperdiet in, iaculis vel ipsum.
              Aliquam erat volutpat.
            </p>
          </div>
          <div class="flex w-full py-12 max-w-6xl mx-auto">
            <div
              class="flex flex-col w-full w-1/4 items-center justify-center icons"
            >
              <img src="/print.svg" />
              <p class="font-bold mt-4">Print Page</p>
            </div>
            <div
              class="flex flex-col w-full w-1/4 items-center justify-center icons"
            >
              <img src="/email.svg" />
              <p class="font-bold mt-4">Email Alerts</p>
            </div>
            <div
              class="flex flex-col w-full w-1/4 items-center justify-center icons"
            >
              <img src="/rss.svg" />
              <p class="font-bold mt-4">RSS</p>
            </div>
            <div
              class="flex flex-col w-full w-1/4 items-center justify-center icons"
            >
              <img src="/question.svg" />
              <p class="font-bold mt-4">Investor FAQ</p>
            </div>
          </div>
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
  </div>
</template>
<style lang="scss">
.tab {
  @apply flex items-center justify-center mr-2 border-b-0;
  background: #eaeaea;
  cursor: pointer;
  &:last-child {
    @apply mr-0;
  }
  &.active {
    background: black;
    border-color: black !important;
    p {
      color: white !important;
    }
  }
}
table {
  width: 100%;
  td {
    @apply text-center py-4;
  }
  tr {
    @apply border-b;
    border-color: #eaeaea;
  }
}
.dataTables_filter,
.dataTables_info,
.dataTables_paginate,
.dataTables_length {
  display: none;
}
</style>
<script>
import $ from "jquery";
import "datatables";
export default {
  mounted() {
    $("table").DataTable();
  },
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
