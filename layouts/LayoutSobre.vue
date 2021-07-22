<template>
  <div>
    <Navbar />
  </div>
</template>
<script>
import Vue from 'vue'
import { BootstrapVue } from 'bootstrap-vue'
import Navbar from '../components/Navbar.vue'
import '../assets/scss/index.css'
Vue.use(BootstrapVue)
export default {
  components: { Navbar }
}
</script>
<style lang="">
</style>
