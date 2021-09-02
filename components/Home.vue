<template>
  <div
    class="py-xs-50 pt-sm-90 pb-sm-50 d-flex align-items-center"
    :class="{
      'bg-home': bgHome,
      'bg-investigacao-conjugal': bgConjugal,
      'bg-investigacao-empresarial': bgEmpresarial,
      'bg-investigacao-politica': bgPolitica,
      'bg-localizacao-de-pessoas': bgLocalizacao,
      'bg-provas': bgProvas,
      'bg-software': bgSoftware,
      'bg-imprensa': bgImprensa
    }"
  >
    <div class="container mt-150">
      <h1 class="text-white text-center position-relative d-flex px-0 justify-content-center col-xl-8 mx-auto text-uppercase fw-400 display-sm-4 display-lg-3 font-teko">
        {{ titleHome }}
        <div class="separation-home" />
      </h1>
      <p class="text-white text-center col-xl-10 px-0 mx-auto mt-45">
        {{ descriptionHome }}
      </p>
      <div class="d-flex mt-4 row mx-auto justify-content-center">
        <button class="btn col-xs-10 btn-lg btn-roxo border-radius-0 px-sm-30 fs-18" @click.prevent="ScrollServicos">
          {{ nameBtnHomeServicos }}
        </button>
        <button class="btn col-xs-10 btn-lg btn-roxo border-radius-0 mt-xs-3 ml-sm-3 px-sm-30 fs-18" @click.prevent="ScrollFooter">
          {{ nameBtnHomeFooter }}
        </button>
      </div>
      <div class="d-flex mt-70 align-items-center">
        <div class="col separation-redes-home mr-4" />
        <div class="d-flex">
          <a href="http://" target="_blank" rel="noopener noreferrer">
            <i class="fab fs-22 text-roxo fa-twitter" />
          </a>
          <a href="http://" target="_blank" class="mx-15" rel="noopener noreferrer">
            <i class="fab fs-22 text-roxo fa-facebook" />
          </a>
          <a href="http://" target="_blank" rel="noopener noreferrer">
            <i class="fab fs-22 text-roxo fa-youtube" />
          </a>
          <a href="http://" target="_blank" class="mx-15" rel="noopener noreferrer">
            <i class="fab fs-22 text-roxo fa-pinterest" />
          </a>
          <a href="http://" target="_blank" rel="noopener noreferrer">
            <i class="fab fs-22 text-roxo fa-instagram" />
          </a>
        </div>
        <div class="col separation-redes-home ml-4" />
      </div>
      <div class="mt-70 bg-roxo-escuro d-flex row mx-auto px-xs-3 px-sm-3 px-lg-30 px-xl-50 py-30">
        <div class="col-xl-4 col-xl-5 px-0 text-white">
          <h3 class="mb-0 text-xs-center text-sm-center text-xl-left">
            <i class="fab fa-telegram-plane mb-1 mr-10 fs-xs-38 fs-sm-38 fs-xl-28 float-xl-left" />
            <div class="text-uppercase font-teko">
              Fale diretamente com uma
              <div class="d-inline-block">
                <div class="position-relative d-flex justify-content-center align-items-center text-roxo-escuro px-1">
                  Mulher
                  <div class="traco-mulher bg-white" />
                  <span class="text-mulher">Mulher</span>
                </div>
              </div>
            </div>
          </h3>
          <p class="mt-1 text-xs-center text-sm-center text-xl-left mb-0">
            Se você não se sente a vontade de falar com um detetive homem você veio ao lugar certo, temos canais de
            atendimento específicos onde você fala com a própria Graziella Bastos!
          </p>
        </div>
        <div class="col-md-11 mx-auto mt-xs-30 mt-sm-30 mt-xl-0 col-xl px-0 text-white d-flex row justify-content-xs-center justify-content-sm-center justify-content-lg-end align-items-center ml-lg-40 ml-xl-50">
          <div class="col-xs-9 col-sm-9 col-md py-10 px-2">
            <div class="d-flex justify-content-center">
              <ion-icon class="fs-37" name="mail-outline" style="margin-top: 0px" />
            </div>
            <p class="fs-13 col-11 mt-1 mb-10 text-center line-height-p-mulher px-0 mx-auto">
              Mande um e-mail
              <br>
              para a Grazi
            </p>
            <div class="d-flex pt-1 justify-content-center">
              <a href="mailto:" class="text-center btn col-12 btn-outline-light border-radius-0 btn-sm">
                Envie seu E-mail <i class="fab fa-telegram-plane ml-1 mb-1" />
              </a>
            </div>
          </div>
          <div class="col-xs-9 col-sm-9 col-md py-10 my-xs-20 my-sm-20 my-md-0 mx-md-40 mx-lg-10 px-2">
            <div class="d-flex justify-content-center">
              <ion-icon class="fs-37" name="call-outline" style="margin-top: 0px" />
            </div>
            <p class="fs-13 col-11 mt-1 mb-10 text-center line-height-p-mulher mx-auto px-0">
              Ligue diretamente
              <br>
              para a Grazi
            </p>
            <div class="d-flex pt-1 justify-content-center">
              <a href="mailto:" class="text-center btn col-12 btn-outline-light border-radius-0 btn-sm">
                Ligue agora <i class="fa fa-phone-alt fs-12 ml-1 mb-1" />
              </a>
            </div>
          </div>
          <div class="col-xs-9 col-sm-9 col-md py-10 px-2">
            <div class="d-flex justify-content-center">
              <ion-icon class="fs-37" name="reader-outline" style="margin-top: 0px" />
            </div>
            <p class="fs-13 col-11 mt-1 mb-10 text-center line-height-p-mulher px-0 mx-auto">
              Preencha nosso
              <br>
              formulário
            </p>
            <div class="d-flex pt-1 justify-content-center">
              <a href="mailto:" class="text-center btn col-12 btn-outline-light border-radius-0 btn-sm">
                Formulário <ion-icon class="fs-16" name="reader-outline" style="margin-bottom: -3px" />
              </a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  props: {
    titleHome: {
      type: String,
      default: 'Acabe com suas suspeitas! Agência Graziella Bastos'
    },
    descriptionHome: {
      type: String,
      default:
      `A Agência de detetives particulares Graziella Bastos está a mais de 15 anos no mercado
      proporcionando para seus clientes investigações de qualidade além de segurança e confidenciabilidade. 
      Conte com a equipe de detetives particulares da Agência de Detetives Graziella Bastos para solucionar
      casos de investigação particular, conjugal, empresarial e muito mais.
      `
    },
    nameBtnHomeServicos: {
      type: String,
      default: 'Nossos serviços'
    },
    nameBtnHomeFooter: {
      type: String,
      default: 'Fale com a Grazi'
    },
    hashBtn: {
      type: String,
      default: '#servicos'
    },
    bgHome: {
      type: Boolean,
      default: false
    },
    bgConjugal: {
      type: Boolean,
      default: false
    },
    bgEmpresarial: {
      type: Boolean,
      default: false
    },
    bgPolitica: {
      type: Boolean,
      default: false
    },
    bgLocalizacao: {
      type: Boolean,
      default: false
    },
    bgProvas: {
      type: Boolean,
      default: false
    },
    bgSoftware: {
      type: Boolean,
      default: false
    },
    bgImprensa: {
      type: Boolean,
      default: false
    }
  },
  data () {
    return {
      Quantidade_retira_hash: 0
    }
  },
  methods: {
    ScrollServicos () {
      this.$smoothScroll({
        scrollTo: document.getElementById('servicos'),
        duration: 500,
        offset: -130
      })
      setTimeout(() => {
        this.HideHash()
      }, 490)
    },
    ScrollFooter () {
      this.$smoothScroll({
        scrollTo: document.getElementById('footer'),
        duration: 500,
        offset: -100
      })
      setTimeout(() => {
        this.HideHash()
      }, 490)
      this.$root.$emit('PulseFooter')
    },
    HideHash () {
      this.Quantidade_retira_hash = 0
      const interval = setInterval(() => {
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
        this.Quantidade_retira_hash++
        if (this.Quantidade_retira_hash > 15) { clearInterval(interval) }
      }, 0)
    }
  }
}
</script>
<style scoped>
  .bg-home{
    background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/bg-home.webp) center center no-repeat;
    -o-background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/bg-home.webp) center center no-repeat;
    -moz-background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/bg-home.webp) center center no-repeat;
    -webkit-background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/bg-home.webp) center center no-repeat;
    background-size: cover;
  }
  .bg-investigacao-conjugal{
    background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/servicos/bg-conjugal.webp) center center no-repeat;
    -o-background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/servicos/bg-conjugal.webp) center center no-repeat;
    -moz-background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/servicos/bg-conjugal.webp) center center no-repeat;
    -webkit-background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/servicos/bg-conjugal.webp) center center no-repeat;
    background-size: cover;
  }
  .bg-investigacao-empresarial{
   background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/servicos/bg-empresarial.webp) center center no-repeat;
    -o-background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/servicos/bg-empresarial.webp) center center no-repeat;
    -moz-background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/servicos/bg-empresarial.webp) center center no-repeat;
    -webkit-background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/servicos/bg-empresarial.webp) center center no-repeat;
    background-size: cover;
  }
  .bg-investigacao-politica{
   background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/servicos/bg-politica.webp) center center no-repeat;
    -o-background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/servicos/bg-politica.webp) center center no-repeat;
    -moz-background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/servicos/bg-politica.webp) center center no-repeat;
    -webkit-background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/servicos/bg-politica.webp) center center no-repeat;
    background-size: cover;
  }
  .bg-localizacao-de-pessoas{
   background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/servicos/bg-localizacao.webp) center center no-repeat;
    -o-background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/servicos/bg-localizacao.webp) center center no-repeat;
    -moz-background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/servicos/bg-localizacao.webp) center center no-repeat;
    -webkit-background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/servicos/bg-localizacao.webp) center center no-repeat;
    background-size: cover;
  }
  .bg-provas{
   background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/servicos/bg-provas.webp) center center no-repeat;
    -o-background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/servicos/bg-provas.webp) center center no-repeat;
    -moz-background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/servicos/bg-provas.webp) center center no-repeat;
    -webkit-background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/servicos/bg-provas.webp) center center no-repeat;
    background-size: cover;
  }
  .bg-software{
   background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/servicos/bg-software.webp) center center no-repeat;
    -o-background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/servicos/bg-software.webp) center center no-repeat;
    -moz-background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/servicos/bg-software.webp) center center no-repeat;
    -webkit-background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/servicos/bg-software.webp) center center no-repeat;
    background-size: cover;
  }
  .bg-imprensa{
   background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/bg-entrevista.webp) center center no-repeat;
    -o-background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/bg-entrevista.webp) center center no-repeat;
    -moz-background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/bg-entrevista.webp) center center no-repeat;
    -webkit-background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/bg-entrevista.webp) center center no-repeat;
    background-size: cover;
  }
  .separation-home{
    position: absolute;
    height: 4px;
    width: 300px;
    bottom: -20px;
    border-radius: 3px;
    background-color: var(--roxo_escuro);
  }
  .traco-mulher{
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 84%;
    z-index: 0;
  }
  @media (min-width: 1200px) {
    .float-xl-left{
      float: left;
    }
  }
  .text-mulher{
    position: absolute;
    z-index: 6 !important;
  }
  .line-height-p-mulher{
    line-height: 14px;
  }
  .separation-redes-home{
    height: 2px;
    border-radius: 3px;
    background-color: var(--roxo_escuro);
  }
</style>
