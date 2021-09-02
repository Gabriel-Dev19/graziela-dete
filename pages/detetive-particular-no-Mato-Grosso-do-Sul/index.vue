<template>
  <div>
    <Home title-home="Detetive particular no Mato Grosso do Sul" :bg-home="true" />
    <section class="pt-100">
      <div class="container">
        <h1 class="font-teko position-relative col-12 px-0 d-flex justify-content-center text-uppercase text-center">
          Contate um detetive particular no Mato Grosso do Sul
          <div class="separation-tema" />
        </h1>
        <p class="mt-35 text-center fw-500 px-0">
          A <b>Agência de Detetives Graziella Bastos</b> está no <b>Mato Grosso do Sul</b> e queremos ajudar você a desvendar suas
          dúvidas. Com mais de 15 anos de experiência e muitos casos resolvidos, atuamos em todo o
          território nacional.
        </p>
        <p class="text-center fw-500 px-0">
          Nossa agência é especializada em investigações de caráter particular, conjugal, empresarial, acompanhamento de
          filhos, localização de bens e pessoas desaparecidas, levantamento de provas para advogados, dentre outras.
          Seja qual for o seu problema e complexidade do caso que você vem enfrentando, a Agência de Detetives
          Graziella Bastos terá a satisfação em ajuda-lo a desvendar.
        </p>
        <div class="d-flex row mx-auto justify-content-center mt-4">
          <btn-roxo-contato-scroll class="col-xs-9" name-btn="Entre em contato" />
          <btn-roxo-footer class="ml-sm-3 mt-xs-2 col-xs-9" />
        </div>
        <h1 class="font-teko d-flex text-center text-uppercase mt-90 justify-content-center position-relative mb-1">
          Confira as cidades atendidas
          <div class="separation-tema" />
        </h1>
      </div>
    </section>
    <section class="col-12 mt-50 px-0">
      <div class="container px-xs-0">
        <!-- Cidades C -->
        <div class="position-relative bg-roxo-escuro border shadow border-radius-10 mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-700 mb-0">
              C
            </h5>
          </div>
          <a class="d-flex col-12 mt-4 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="CampoGrande">
            <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Campo Grande – MS
          </a>
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
    title: 'Detetive particular no Mato Grosso do Sul - Agência de detetives Graziella Bastos'
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
    CampoGrande () {
      this.$router.push('/detetive-particular-no-Mato-Grosso-do-Sul/detetive-particular-em-Campo-Grande-MS/')
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
