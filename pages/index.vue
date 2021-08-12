<template>
  <div>
    <Navbar />
    <Home :bg-home="true" />
    <Planejamento />
    <Servicos />
    <ParalaxHome />
    <Numeros />
    <Motivos />
    <Comentarios />
    <Perguntas />
    <Contato />
    <Footer />
  </div>
</template>

<script>
import Home from '~/components/Home.vue'
import Navbar from '~/components/Navbar.vue'
import Planejamento from '~/components/Planejamento.vue'
import Servicos from '~/components/Servicos.vue'
import ParalaxHome from '~/components/ParalaxHome.vue'
import Numeros from '~/components/Numeros.vue'
import Motivos from '~/components/Motivos.vue'
import Comentarios from '~/components/Comentarios.vue'
import Perguntas from '~/components/Perguntas.vue'
import Contato from '~/components/Contato.vue'
import Footer from '~/components/Footer.vue'
export default {
  components: {
    Navbar,
    Home,
    Planejamento,
    Servicos,
    ParalaxHome,
    Numeros,
    Motivos,
    Comentarios,
    Perguntas,
    Contato,
    Footer
  },
  mounted () {
    this.$smoothScroll({
      scrollTo: document.body,
      duration: 0,
      offset: 0
    })
    this.HideHash()
  },
  methods: {
    HideHash () {
      let scrollV; let scrollH; const loc = window.location
      if ('replaceState' in history) {
        history.replaceState('', document.title, loc.pathname + loc.search)
      } else {
        // Prevent scrolling by storing the page's current scroll offset
        scrollV = document.body.scrollTop
        scrollH = document.body.scrollLeft
        loc.hash = ''
        // Restore the scroll offset, should be flicker free
        document.body.scrollTop = scrollV
        document.body.scrollLeft = scrollH
      }
    }
  }
}
</script>
