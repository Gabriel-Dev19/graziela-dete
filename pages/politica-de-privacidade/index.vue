<template>
  <div>
    <Home title-home="Políticas de privacidade e Cookies" :bg-home="true" />
    <section class="pt-100">
      <div class="container">
        <h1 class="font-teko position-relative col-12 px-0 d-flex justify-content-center text-uppercase text-center">
          Políticas de privacidade e Cookies
          <div class="separation-tema" />
        </h1>
        <p class="mt-35 text-center fw-500 px-0">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Animi ipsam consequatur modi rem voluptas molestias
          omnis sed iusto veniam error? Nostrum quaerat inventore earum commodi nihil, et ad mollitia voluptatem.
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Animi ipsam consequatur modi rem voluptas molestias
          omnis sed iusto veniam error? Nostrum quaerat inventore earum commodi nihil, et ad mollitia voluptatem.
        </p>
        <div class="d-flex row mx-auto justify-content-center mt-4">
          <btn-roxo-contato-scroll class="col-xs-9" name-btn="Entre em contato" />
          <btn-roxo-footer class="ml-sm-3 mt-xs-2 col-xs-9" />
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import BtnRoxoContatoScroll from '~/components/buttons/BtnRoxoContatoScroll.vue'
import BtnRoxoFooter from '~/components/buttons/BtnRoxoFooter.vue'
import Home from '~/components/Home.vue'
export default {
  components: { Home, BtnRoxoContatoScroll, BtnRoxoFooter },
  layout: 'LayoutSobre',
  head: {
    title: 'Políticas de privacidade - Agência de detetives Graziella Bastos'
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
    },
    SaoPaulo () {
      this.$router.push('/detetive-particular-em-Sao-Paulo/detetive-particular-em-Sao-Paulo-SP/')
    }
  }
}
</script>
<style scoped>
  .separation-tema{
    position: absolute;
    height: 3px;
    width: 200px;
    bottom: -10px;
    border-radius: 3px;
    background-color: var(--roxo_escuro);
  }
  .borda-tema-fina{
    position: absolute;
    height: 2px;
    width: 200px;
    bottom: -1px;
    border-radius: 3px;
    background-color: var(--roxo_escuro);
  }
  ol.carousel-indicators li{
    width: 13px !important;
    height: 13px !important;
  }
</style>
