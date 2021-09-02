<template>
  <div>
    <Home title-home="Detetive particular no estado do Paraná" :bg-home="true" />
    <section class="pt-100">
      <div class="container">
        <h1 class="font-teko position-relative col-12 px-0 d-flex justify-content-center text-uppercase text-center">
          Contate um detetive particular no Paraná
          <div class="separation-tema" />
        </h1>
        <p class="mt-35 text-center fw-500 px-0">
          A <b>Agência de Detetives Graziella Bastos</b> está no <b>Paraná</b> e queremos ajudar você a desvendar suas
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
        <!-- Cidades A -->
        <div class="position-relative bg-roxo-escuro border shadow border-radius-10 overflow-hidden mt-30 col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-700 mb-1">
              A
            </h5>
          </div>
          <div class="col-lg px-0 mt-4">
            <a class="d-flex col-auto px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Adrianopolis">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Adrianópolis - PR
            </a>
            <a class="d-flex col-auto px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="AgudosDoSul">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Agudos do Sul - PR
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-auto px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Antonina">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Antonina - PR
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-auto px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Araucaria">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Araucária - PR
            </a>
          </div>
        </div>
        <!-- Cidades B -->
        <div class="position-relative bg-roxo-escuro border shadow border-radius-10 mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-700 mb-0">
              B
            </h5>
          </div>
          <a class="d-flex col-12 mt-4 px-0 py-0 mt-1 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="BalsaNova">
            <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Balsa Nova - PR
          </a>
          <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="BocaiuvaDoSul">
            <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Bocaiuva do Sul - PR
          </a>
        </div>
        <!-- Cidades C -->
        <div class="position-relative bg-roxo-escuro border shadow border-radius-10 mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-700 mb-0">
              C
            </h5>
          </div>
          <div class="col-lg px-0 mt-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="CampoDoTenente">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Campo do Tenente – PR
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="CampoLargo">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Campo Largo – PR
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Cascavel">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Cascavel – PR
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="CampinaGrandeDoSul">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Campina Grande do Sul – PR
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="CampoMagro">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Campo Magro – PR
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="CerroAzul">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Cerro Azul – PR
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Contenda">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Contenda – PR
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Curitiba">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Curitiba – PR
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Colombo">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Colombo – PR
            </a>
          </div>
        </div>
        <!-- Cidades D -->
        <div class="position-relative bg-roxo-escuro border shadow border-radius-10 mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-700 mb-0">
              D
            </h5>
          </div>
          <div class="col-lg mt-4 px-0">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="DoutorUlysses">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Doutor Ulysses – PR
            </a>
          </div>
        </div>
        <!-- Cidades F -->
        <div class="position-relative bg-roxo-escuro border shadow border-radius-10 mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-700 mb-0">
              F
            </h5>
          </div>
          <a class="d-flex col-12 mt-4 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="FozDoIguacu">
            <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Foz do Iguaçu – PR
          </a>
          <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="FazendaRioGrande">
            <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Fazenda Rio Grande – PR
          </a>
        </div>
        <!-- Cidades G -->
        <div class="position-relative bg-roxo-escuro border shadow border-radius-10 mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-700 mb-0">
              G
            </h5>
          </div>
          <a class="d-flex mt-4 col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Guaraquecaba">
            <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Guaraqueçaba – PR
          </a>
          <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Guaratuba">
            <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Guaratuba – PR
          </a>
        </div>
        <!-- Cidades I -->
        <div class="position-relative bg-roxo-escuro border shadow border-radius-10 mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-700 mb-0">
              I
            </h5>
          </div>
          <a class="d-flex col-12 mt-4 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Itaperucu">
            <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Itaperuçu – PR
          </a>
        </div>
        <!-- Cidades L -->
        <div class="position-relative bg-roxo-escuro border shadow border-radius-10 mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-700 mb-0">
              L
            </h5>
          </div>
          <a class="d-flex mt-4 col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Lapa">
            <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Lapa – PR
          </a>
          <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Londrina">
            <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Londrina – PR
          </a>
        </div>
        <!-- Cidades M -->
        <div class="position-relative bg-roxo-escuro border shadow border-radius-10 mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-700 mb-0">
              M
            </h5>
          </div>
          <div class="col-lg px-0 mt-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Mandirituba">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Mandirituba – PR
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Matinhos">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Matinhos – PR
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Maringa">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Maringá – PR
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Morretes">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Morretes – PR
            </a>
          </div>
        </div>
        <!-- Cidades P -->
        <div class="position-relative bg-roxo-escuro border shadow border-radius-10 mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-700 mb-0">
              P
            </h5>
          </div>
          <div class="col-lg px-0 mt-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Pinhais">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Pinhais – PR
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Piraquara">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Piraquara – PR
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="PontalDoParana">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Pontal do Paraná – PR
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="PontaGrossa">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Ponta Grossa – PR
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Paranagua">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Paranaguá – PR
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Piên">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Piên – PR
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="PatoBranco">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Pato Branco – PR
            </a>
          </div>
        </div>
        <!-- Cidades Q -->
        <div class="position-relative bg-roxo-escuro border shadow border-radius-10 mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-700 mb-0">
              Q
            </h5>
          </div>
          <a class="d-flex col-12 mt-4 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Quitandinha">
            <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Quitandinha – PR
          </a>
          <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="QuatroBarras">
            <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Quatro Barras – PR
          </a>
        </div>
        <!-- Cidades R -->
        <div class="position-relative bg-roxo-escuro border shadow border-radius-10 mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-700 mb-0">
              R
            </h5>
          </div>
          <a class="d-flex col-12 mt-4 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="RioBrancoDoSul">
            <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Rio Branco do Sul – PR
          </a>
        </div>
        <!-- Cidades S -->
        <div class="position-relative bg-roxo-escuro border shadow border-radius-10 mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-700 mb-0">
              S
            </h5>
          </div>
          <a class="d-flex col-12 mt-4 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="SaoJoseDosPinhais">
            <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> São José dos Pinhais – PR
          </a>
        </div>
        <!-- Cidades T -->
        <div class="position-relative bg-roxo-escuro border shadow border-radius-10 mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-700 mb-0">
              T
            </h5>
          </div>
          <a class="d-flex col-12 mt-4 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="TijucasDoSul">
            <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Tijucas do Sul – PR
          </a>
          <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="TunasDoParana">
            <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Tunas do Paraná – PR
          </a>
          <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Toledo">
            <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Toledo – PR
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
    title: 'Detetive particular no Paraná - Agência de detetives Graziella Bastos'
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
    Adrianopolis () {
      this.$router.push('/detetive-particular-no-Parana/detetive-particular-em-Adrianopolis-PR/')
    },
    AgudosDoSul () {
      this.$router.push('/detetive-particular-no-Parana/detetive-particular-em-Agudos-do-Sul-PR/')
    },
    Antonina () {
      this.$router.push('/detetive-particular-no-Parana/detetive-particular-em-Antonina-PR/')
    },
    Araucaria () {
      this.$router.push('/detetive-particular-no-Parana/detetive-particular-em-Araucaria-PR/')
    },
    BalsaNova () {
      this.$router.push('/detetive-particular-no-Parana/detetive-particular-em-Balsa-Nova-PR/')
    },
    BocaiuvaDoSul () {
      this.$router.push('/detetive-particular-no-Parana/detetive-particular-em-Bocaiuva-do-Sul-PR/')
    },
    CampoDoTenente () {
      this.$router.push('/detetive-particular-no-Parana/detetive-particular-em-Campo-do-Tenente-PR/')
    },
    CampoLargo () {
      this.$router.push('/detetive-particular-no-Parana/detetive-particular-em-Campo-Largo-PR/')
    },
    Cascavel () {
      this.$router.push('/detetive-particular-no-Parana/detetive-particular-em-Cascavel-PR/')
    },
    CampinaGrandeDoSul () {
      this.$router.push('/detetive-particular-no-Parana/detetive-particular-em-Campina-Grande-do-Sul-PR/')
    },
    CampoMagro () {
      this.$router.push('/detetive-particular-no-Parana/detetive-particular-em-Campo-Magro-PR/')
    },
    CerroAzul () {
      this.$router.push('/detetive-particular-no-Parana/detetive-particular-em-Cerro-Azul-PR/')
    },
    Contenda () {
      this.$router.push('/detetive-particular-no-Parana/detetive-particular-em-Contenda-PR/')
    },
    Curitiba () {
      this.$router.push('/detetive-particular-no-Parana/detetive-particular-em-Curitiba-PR/')
    },
    Colombo () {
      this.$router.push('/detetive-particular-no-Parana/detetive-particular-em-Colombo-PR/')
    },
    DoutorUlysses () {
      this.$router.push('/detetive-particular-no-Parana/detetive-particular-em-Doutor-Ulysses-PR/')
    },
    FozDoIguacu () {
      this.$router.push('/detetive-particular-no-Parana/detetive-particular-em-Foz-do-Iguacu-PR/')
    },
    FazendaRioGrande () {
      this.$router.push('/detetive-particular-no-Parana/detetive-particular-em-Fazenda-Rio-Grande-PR/')
    },
    Guaraquecaba () {
      this.$router.push('/detetive-particular-no-Parana/detetive-particular-em-Guaraquecaba-PR/')
    },
    Guaratuba () {
      this.$router.push('/detetive-particular-no-Parana/detetive-particular-em-Guaratuba-PR/')
    },
    Itaperucu () {
      this.$router.push('/detetive-particular-no-Parana/detetive-particular-em-Itaperucu-PR/')
    },
    Lapa () {
      this.$router.push('/detetive-particular-no-Parana/detetive-particular-em-Lapa-PR/')
    },
    Londrina () {
      this.$router.push('/detetive-particular-no-Parana/detetive-particular-em-Londrina-PR/')
    },
    Mandirituba () {
      this.$router.push('/detetive-particular-no-Parana/detetive-particular-em-Mandirituba-PR/')
    },
    Matinhos () {
      this.$router.push('/detetive-particular-no-Parana/detetive-particular-em-Matinhos-PR/')
    },
    Maringa () {
      this.$router.push('/detetive-particular-no-Parana/detetive-particular-em-Maringa-PR/')
    },
    Morretes () {
      this.$router.push('/detetive-particular-no-Parana/detetive-particular-em-Morretes-PR/')
    },
    Pinhais () {
      this.$router.push('/detetive-particular-no-Parana/detetive-particular-em-Pinhais-PR/')
    },
    Piraquara () {
      this.$router.push('/detetive-particular-no-Parana/detetive-particular-em-Piraquara-PR/')
    },
    PontalDoParana () {
      this.$router.push('/detetive-particular-no-Parana/detetive-particular-em-Pontal-do-Parana-PR/')
    },
    PontaGrossa () {
      this.$router.push('/detetive-particular-no-Parana/detetive-particular-em-Ponta-Grossa-PR/')
    },
    Paranagua () {
      this.$router.push('/detetive-particular-no-Parana/detetive-particular-em-Paranagua-PR/')
    },
    Piên () {
      this.$router.push('/detetive-particular-no-Parana/detetive-particular-em-Pien-PR/')
    },
    PatoBranco () {
      this.$router.push('/detetive-particular-no-Parana/detetive-particular-em-Pato-Branco-PR/')
    },
    Quitandinha () {
      this.$router.push('/detetive-particular-no-Parana/detetive-particular-em-Quitandinha-PR/')
    },
    QuatroBarras () {
      this.$router.push('/detetive-particular-no-Parana/detetive-particular-em-Quatro-Barras-PR/')
    },
    RioBrancoDoSul () {
      this.$router.push('/detetive-particular-no-Parana/detetive-particular-em-Rio-Branco-do-Sul-PR/')
    },
    SaoJoseDosPinhais () {
      this.$router.push('/detetive-particular-no-Parana/detetive-particular-em-Sao-Jose-dos-Pinhais-PR/')
    },
    TijucasDoSul () {
      this.$router.push('/detetive-particular-no-Parana/detetive-particular-em-Tijucas-do-Sul-PR/')
    },
    TunasDoParana () {
      this.$router.push('/detetive-particular-no-Parana/detetive-particular-em-Tunas-do-Parana-PR/')
    },
    Toledo () {
      this.$router.push('/detetive-particular-no-Parana/detetive-particular-em-Toledo-PR/')
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
