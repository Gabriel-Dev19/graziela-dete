<template>
  <div>
    <Nuxt />
    <BtnVoltarTopo />
    <BtnWhatsappFlutuante />
    <ModalWhatsapp />
  </div>
</template>
<script>
import Vue from '../node_modules/vue'
import VueSmoothScroll from '../node_modules/vue2-smooth-scroll'
import BtnVoltarTopo from '~/components/buttons/BtnVoltarTopo.vue'
import BtnWhatsappFlutuante from '~/components/buttons/BtnWhatsappFlutuante.vue'
import ModalWhatsapp from '~/components/ModalWhatsapp.vue'
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
  components: { BtnVoltarTopo, BtnWhatsappFlutuante, ModalWhatsapp }

}
</script>
