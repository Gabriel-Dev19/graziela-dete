<template>
  <div>
    <Home title-home="Comportamento de filhos - atitudes suspeitas" name-btn-home-servicos="Outros serviços" :bg-comportamento="true" />
    <section class="pt-100">
      <div class="container">
        <h1 class="font-teko position-relative col-12 px-0 d-flex justify-content-center text-uppercase text-center">
          Mais sobre Comportamento de filhos
          <div class="separation-tema" />
        </h1>
        <div class="mt-50 row mx-auto d-xs-flex d-sm-block">
          <div class="col-sm-5 col-md-4 col-lg-3 px-0 mt-xs-50 ml-sm-30 mb-sm-30 order-2 float-sm-right">
            <h5 class="fw-600 text-xs-center text-roxo-escuro">
              Investigação com riqueza de detalhes!
            </h5>
            <p class="fs-14 text-xs-center fw-500">
              Detalhamos a investigação completa e fornecemos
              tudo documentado.
            </p>
            <div class="position-relative">
              <div class="borda-lateral-sobre d-xs-none" />
              <div class="d-flex row mx-auto justify-content-xs-center">
                <ion-icon class="fs-24 bg-light order-xs-2 mt-xs-1 text-roxo-escuro" name="chevron-down-circle-outline" style="margin-top: -2px; --ionicon-stroke-width: 23px;" />
                <span class="fs-14 col-xs-12 text-xs-center order-xs-1 fw-500 ml-1">Diagnóstico</span>
              </div>
              <div class="d-flex row mx-auto justify-content-xs-center mt-15">
                <ion-icon class="fs-24 bg-light order-xs-2 mt-xs-1 text-roxo-escuro" name="chevron-down-circle-outline" style="margin-top: -2px; --ionicon-stroke-width: 23px;" />
                <span class="fs-14 col-xs-12 text-xs-center order-xs-1 fw-500 ml-1">Planejamento</span>
              </div>
              <div class="d-flex row mx-auto justify-content-xs-center mt-15">
                <ion-icon class="fs-24 bg-light order-xs-2 mt-xs-1 text-roxo-escuro" name="chevron-down-circle-outline" style="margin-top: -2px; --ionicon-stroke-width: 23px;" />
                <span class="fs-14 col-xs-12 text-xs-center order-xs-1 fw-500 ml-1">Investigação</span>
              </div>
              <div class="d-flex row mx-auto justify-content-xs-center mt-15">
                <ion-icon class="fs-24 bg-light order-xs-2 mt-xs-1 text-roxo-escuro" name="chevron-down-circle-outline" style="margin-top: -2px; --ionicon-stroke-width: 23px;" />
                <span class="fs-14 col-xs-12 text-xs-center order-xs-1 fw-500 ml-1">Coleta de provas</span>
              </div>
              <div class="d-flex row mx-auto justify-content-xs-center mt-15">
                <ion-icon class="fs-24 bg-light order-xs-2 mt-xs-1 text-roxo-escuro" name="chevron-down-circle-outline" style="margin-top: -2px; --ionicon-stroke-width: 23px;" />
                <span class="fs-14 col-xs-12 text-xs-center order-xs-1 fw-500 ml-1">Preparação do dossiê</span>
              </div>
              <div class="d-flex row mx-auto justify-content-xs-center mt-15">
                <ion-icon class="fs-24 bg-light order-xs-2 mt-xs-1 text-roxo-escuro" name="checkmark-circle" style="margin-top: -2px; --ionicon-stroke-width: 23px;" />
                <span class="fs-14 col-xs-12 text-xs-center order-xs-1 fw-500 ml-1">A verdade nas suas mãos!</span>
              </div>
            </div>
            <div class="d-flex justify-content-xs-center">
              <BtnRoxoContatoScroll class="mt-4" name-btn="Faça uma consulta" />
            </div>
          </div>
          <p class="fw-500 col-xs-12 px-0 text-xs-center text-sm-left">
            O comportamento dos filhos pode mudar à medida que eles adquirirem certa independência. Alguns podem desenvolver a habilidade de mentir e enganar os pais quanto aos locais que frequentam, companhias e atividades. Por influência de amigos, redes sociais e outros adultos eles podem se envolver em atividades criminosas ou ilegais.
          </p>
          <p class="fw-500 col-xs-12 px-0 text-xs-center text-sm-left">
            Atos de rebeldia, como pequenos furtos ou vandalismo podem ser o resultado da busca por “emoção” e autoafirmação dos pré-adolescentes e adolescentes. Embora muitos desses delitos não sejam graves — ou não venham se tornar parte da vida dos filhos — os pais devem estar atentos para prevenirem o risco de isso acontecer.
          </p>
          <p class="fw-500 col-xs-12 px-0 text-xs-center text-sm-left">
            Foi pensando em cuidar da proteção da sua família que a Agência de Detetives Graziella Bastos idealizou o serviço de Detetive Particular voltado ao monitoramento do comportamento dos filhos. Crianças ou adolescentes acreditam estar acima de todos os perigos que o mundo lhes reserva, devido à pouca experiência de vida que têm.
          </p>
        </div>
      </div>
    </section>
    <Servicos title-servicos="Outros serviços" class="mt-150" :hide-comportamento="false" />
  </div>
</template>

<script>
import BtnRoxoContatoScroll from '~/components/buttons/BtnRoxoContatoScroll.vue'
import Home from '~/components/Home.vue'
import Servicos from '~/components/Servicos.vue'
export default {
  components: { Home, Servicos, BtnRoxoContatoScroll },
  layout: 'LayoutServicos',
  head: {
    title: 'Comportamento de filhos - Agência de detetives Graziella Bastos'
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
  .borda-lateral-sobre{
    position: absolute;
    height: 100%;
    top: 0;
    left: 12px;
    z-index: -3;
    border-left: 1px solid var(--roxo_escuro);
  }
</style>
