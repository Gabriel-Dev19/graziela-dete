<template>
  <div>
    <Navbar />
    <Nuxt />
    <ParalaxHome />
    <Numeros />
    <Contato />
    <Footer />
    <ModalWhatsapp />
    <BtnVoltarTopo />
    <BtnWhatsappFlutuante />
    <client-only>
      <Cookies />
    </client-only>
  </div>
</template>
<script>
import VueSmoothScroll from '../node_modules/vue2-smooth-scroll'
import Vue from '~/node_modules/vue'
import Navbar from '~/components/Navbar.vue'
import BtnVoltarTopo from '~/components/buttons/BtnVoltarTopo.vue'
import ParalaxHome from '~/components/ParalaxHome.vue'
import Numeros from '~/components/Numeros.vue'
import Contato from '~/components/Contato.vue'
import Footer from '~/components/Footer.vue'
import ModalWhatsapp from '~/components/ModalWhatsapp.vue'
import Cookies from '~/components/Cookies.vue'
import BtnWhatsappFlutuante from '~/components/buttons/BtnWhatsappFlutuante.vue'
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
  components: {
    Navbar,
    BtnVoltarTopo,
    ParalaxHome,
    Numeros,
    Contato,
    Footer,
    ModalWhatsapp,
    Cookies,
    BtnWhatsappFlutuante
  }
}
</script>
<style scoped>

</style>
