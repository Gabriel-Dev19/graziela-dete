<template>
  <div>
    <Navbar />
    <Nuxt />
    <btn-voltar-topo />
  </div>
</template>
<script>
import Vue from '../node_modules/vue'
import Navbar from '../components/Navbar.vue'
import VueSmoothScroll from '../node_modules/vue2-smooth-scroll'
import BtnVoltarTopo from '~/components/buttons/BtnVoltarTopo.vue'
Vue.use(VueSmoothScroll)
Vue.directive('scroll', {
  inserted (el, binding) {
    const f = function (evt) {
      if (binding.value(evt, el)) {
        window.removeEventListener('scroll', f)
      }
    }
    window.addEventListener('scroll', f)
  }
})
export default {
  components: { Navbar, BtnVoltarTopo }
}
</script>
<style lang="">
</style>
