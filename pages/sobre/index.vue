<template>
  <div>
    <Home title-home="Sobre a agência Graziella Bastos" :bg-home="true" />
    <section class="pt-100">
      <div class="container">
        <h1 class="font-teko position-relative col-12 px-0 d-flex justify-content-center text-uppercase text-center">
          Saiba mais sobre Graziella e sua equipe
          <div class="separation-tema" />
        </h1>
        <div class="d-flex justify-content-between align-items-start row mx-auto mt-80">
          <div class="col-lg-6 col-xl-7 px-0">
            <h1 class="font-teko d-flex justify-content-xs-center justify-content-sm-center justify-content-lg-start position-relative mb-1">
              O que fazemos?
              <div class="borda-tema-fina" />
            </h1>
            <p class="mt-3 text-xs-center text-sm-center text-lg-left fw-500 px-0">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Animi ipsam consequatur modi rem voluptas molestias
              omnis sed iusto veniam error? Nostrum quaerat inventore earum commodi nihil, et ad mollitia voluptatem.
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Animi ipsam consequatur modi rem voluptas molestias
              omnis sed iusto veniam error? Nostrum quaerat inventore earum commodi nihil, et ad mollitia voluptatem.
            </p>
            <h1 class="font-teko mt-30 d-flex justify-content-xs-center justify-content-sm-center justify-content-lg-start position-relative position-relative mb-1">
              Nossa equipe
              <div class="borda-tema-fina" />
            </h1>
            <p class="mt-3 text-xs-center text-sm-center text-lg-left fw-500 px-0">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Animi ipsam consequatur modi rem voluptas molestias
              omnis sed iusto veniam error? Nostrum quaerat inventore earum commodi nihil, et ad mollitia voluptatem.
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Animi ipsam consequatur modi rem voluptas molestias
              omnis sed iusto veniam error? Nostrum quaerat inventore earum commodi nihil, et ad mollitia voluptatem.
            </p>
            <div class="d-flex justify-content-xs-center justify-content-sm-center mt-4 justify-content-lg-start">
              <btn-roxo-contato-scroll name-btn="Entre em contato" />
            </div>
          </div>
          <div class="col-lg ml-lg-90 mt-xs-70 mt-sm-70 mt-lg-0 px-0">
            <card-sobre />
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import BtnRoxoContatoScroll from '~/components/buttons/BtnRoxoContatoScroll.vue'
import Home from '~/components/Home.vue'
import CardSobre from '~/components/parts/CardSobre.vue'
export default {
  components: { Home, BtnRoxoContatoScroll, CardSobre },
  layout: 'LayoutSobre',
  head: {
    title: 'Sobre nós - Agência de detetives Graziella Bastos'
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
