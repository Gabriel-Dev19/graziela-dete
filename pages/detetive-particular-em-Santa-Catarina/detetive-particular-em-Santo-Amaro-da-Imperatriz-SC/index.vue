<template>
  <div>
    <Home title-home="Detetive particular em Santo Amaro da Imperatriz - SC" :bg-home="true" />
    <Cidades name-cidades="Santo Amaro da Imperatriz - SC" :show-quatro-oito="true" />
  </div>
</template>

<script>
import Home from '~/components/Home.vue'
import Cidades from '~/components/parts/Cidades.vue'
export default {
  components: { Home, Cidades },
  layout: 'LayoutSobre',
  head: {
    title: 'Detetive particular em Santo Amaro da Imperatriz - SC - Agência de detetives Graziella Bastos'
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
