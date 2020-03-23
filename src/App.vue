<template>
  <div id="app">
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
  }
}
</script>
