<template>
  <div id="app">
      <!-- Sidebar -->
      <b-nav vertical pills class="sidenav h-100 pt-3 pl-3 text-white">
          <b-nav-item class="pb-3" to="#dashboard" :active='dashboard' v-on:click='sidebar_click("dashboard")'>Dashboard</b-nav-item>
          <b-nav-item class="pb-3" to="#products" :active='products' v-on:click='sidebar_click("products")'>Products</b-nav-item>
          <b-nav-item class="pb-3" to="#penjualan" :active='penjualan' v-on:click='sidebar_click("penjualan")'>Penjualan</b-nav-item>
          <b-nav-item class="pb-3" to="#pembelian" :active='pembelian' v-on:click='sidebar_click("pembelian")'>Pembelian</b-nav-item>
    </b-nav>
    <Test msg="Elit ad consequat sunt labore duis id cupidatat ea ipsum pariatur laborum mollit. Laborum do eiusmod et magna non velit adipisicing aliqua labore. Ad ea ut et non adipisicing amet sint do quis. Commodo do consequat eu aliquip est labore officia et nostrud laboris esse voluptate."/>
  </div>
</template>

<script>
  import Test from './components/Test.vue'
  import Vue from 'vue'
  import { BootstrapVue, IconsPlugin } from 'bootstrap-vue'

  // Install BootstrapVue
  Vue.use(BootstrapVue)
  // Optionally install the BootstrapVue icon components plugin
  Vue.use(IconsPlugin)

  export default {
    name: 'App',
    components: {
      Test
    },
    methods: {      
      sidebar_click: function(hash) {
        let dt;
        switch(hash) {
          case "dashboard":
            for (dt in this.$data) this.$data[dt] = false;
            this.$data.dashboard = true;
            break;
          case "products":
            for (dt in this.$data) this.$data[dt] = false;
            this.$data.products = true;
            break;
          case "penjualan":
            for (dt in this.$data) this.$data[dt] = false;
            this.$data.penjualan = true;
            break;
          case "pembelian":
            for (dt in this.$data) 
              this.$data[dt] = false;
            this.$data.pembelian = true;
            break;
        }
      }
    },
    data: function() {
      return {
        dashboard: true,
        products: false,
        penjualan: false,
        pembelian: false
      }
    }
  }
</script>
