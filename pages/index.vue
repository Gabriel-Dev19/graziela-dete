<template>
  <div>
    <Navbar />
    <Home bg-home="true" />
    <Planejamento />
    <Servicos />
    <ParalaxHome />
    <Numeros />
    <Motivos />
    <section class="height-100-vh" />
  </div>
</template>

<script>
import Vue from '../node_modules/vue'
import Home from '~/components/Home.vue'
import Navbar from '~/components/Navbar.vue'
import Planejamento from '~/components/Planejamento.vue'
import Servicos from '~/components/Servicos.vue'
import ParalaxHome from '~/components/ParalaxHome.vue'
import Numeros from '~/components/Numeros.vue'
import Motivos from '~/components/Motivos.vue'
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
  components: { Navbar, Home, Planejamento, Servicos, ParalaxHome, Numeros, Motivos }
}
</script>
