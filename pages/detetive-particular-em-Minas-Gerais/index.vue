<template>
  <div>
    <Home title-home="Detetive particular em Minas Gerais" :bg-home="true" />
    <section class="pt-100">
      <div class="container">
        <h1 class="font-teko position-relative col-12 px-0 d-flex justify-content-center text-uppercase text-center">
          Contate um detetive particular em Minas Gerais
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
        <h1 class="font-teko d-flex text-center text-uppercase mt-90 justify-content-center position-relative mb-1">
          Confira as cidades atendidas
          <div class="borda-tema-fina" />
        </h1>
      </div>
    </section>
    <section class="col-12 px-0">
      <div class="container px-xs-0">
        <!-- Cidades B -->
        <div class="position-relative bg-roxo-escuro border shadow border-radius-10 mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-700 mb-0">
              B
            </h5>
          </div>
          <a class="d-flex col-12 mt-4 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="BeloHorizonte">
            <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Belo Horizonte – MG
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
    title: 'Detetive particular em Minas Gerais - Agência de detetives Graziella Bastos'
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
    BeloHorizonte () {
      this.$router.push('/detetive-particular-em-Minas-Gerais/detetive-particular-em-Belo-Horizonte-MG/')
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
    background-color: var(--roxo);
  }
  .borda-tema-fina{
    position: absolute;
    height: 2px;
    width: 200px;
    bottom: -1px;
    border-radius: 3px;
    background-color: var(--roxo);
  }
  ol.carousel-indicators li{
    width: 13px !important;
    height: 13px !important;
  }
</style>
