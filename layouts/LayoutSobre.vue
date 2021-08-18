<template>
  <div>
    <Navbar />
    <Nuxt />
    <Servicos class="mt-150" />
    <ParalaxHome />
    <Numeros />
    <Contato />
    <Footer />
    <ModalWhatsapp />
    <BtnVoltarTopo />
  </div>
</template>
<script>
import Vue from '../node_modules/vue'
import Navbar from '../components/Navbar.vue'
import VueSmoothScroll from '../node_modules/vue2-smooth-scroll'
import BtnVoltarTopo from '~/components/buttons/BtnVoltarTopo.vue'
import Contato from '~/components/Contato.vue'
import Footer from '~/components/Footer.vue'
import Numeros from '~/components/Numeros.vue'
import ParalaxHome from '~/components/ParalaxHome.vue'
import Servicos from '~/components/Servicos.vue'
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
  components: { Navbar, BtnVoltarTopo, Servicos, ParalaxHome, Numeros, Contato, Footer, ModalWhatsapp }
}
</script>
<style lang="">
</style>
