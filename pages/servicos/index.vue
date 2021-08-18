<template>
  <div>
    <Home title-home="Serviços de detetive particular" :bg-home="true" />
    <Servicos />
    <ParalaxHome />
    <Numeros />
    <Contato />
    <Footer />
  </div>
</template>

<script>
import Contato from '~/components/Contato.vue'
import Footer from '~/components/Footer.vue'
import Home from '~/components/Home.vue'
import Numeros from '~/components/Numeros.vue'
import ParalaxHome from '~/components/ParalaxHome.vue'
import Servicos from '~/components/Servicos.vue'
export default {
  components: { Home, Servicos, ParalaxHome, Numeros, Contato, Footer },
  layout: 'LayoutServicos',
  head: {
    title: 'Serviços - Agência de detetives Graziella Bastos'
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
