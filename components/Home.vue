<template>
  <div
    class="py-xs-50 pt-sm-90 pb-sm-50 d-flex align-items-center"
    :class="{
      'bg-home': bgHome,
      'bg-investigacao-conjugal': bgConjugal,
      'bg-investigacao-empresarial': bgEmpresarial,
      'bg-investigacao-politica': bgPolitica,
      'bg-localizacao-de-pessoas': bgLocalizacao, }"
  >
    <div class="container mt-110">
      <h1 class="text-white text-center position-relative d-flex px-0 justify-content-center col-xl-8 mx-auto text-uppercase fw-400 display-sm-4 display-lg-3 font-teko">
        {{ titleHome }}
        <div class="separation-home" />
      </h1>
      <p class="text-white text-center col-xl-10 px-0 mx-auto mt-45">
        {{ descriptionHome }}
      </p>
      <div class="d-flex mt-4 row mx-auto justify-content-center">
        <a :href="hashBtn" class="btn col-xs-10 btn-lg btn-roxo border-radius-0 px-sm-30 fs-18">
          {{ nameBtnHomeServicos }}
        </a>
        <a :href="hashBtn" class="btn col-xs-10 btn-lg btn-roxo border-radius-0 mt-xs-3 ml-sm-3 px-sm-30 fs-18">
          {{ nameBtnHomeContact }}
        </a>
      </div>
      <div class="d-flex mt-70 align-items-center">
        <div class="col separation-redes-home mr-3" />
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
        <div class="col separation-redes-home ml-3" />
      </div>
      <div class="mt-70 bg-roxo-escuro d-flex row mx-auto px-xs-3 px-sm-3 px-lg-30 px-xl-50 py-30">
        <div class="col-lg-4 col-xl-5 px-0 text-white">
          <h3 class="mb-0 text-xs-center text-sm-center text-lg-left">
            <i class="fab fa-telegram-plane mb-1 mr-10 fs-xs-35 fs-sm-35 fs-lg-28 float-lg-left" />
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
          <p class="mt-1 text-xs-center text-sm-center text-lg-left mb-0">
            Se você não se sente a vontade de falar com um detetive homem você veio ao lugar certo, temos canais de
            atendimento específicos onde você fala com a própria Graziela Bastos!
          </p>
        </div>
        <div class="col-md-11 mx-auto mt-xs-30 mt-sm-30 mt-lg-0 col-lg px-0 text-white d-flex row justify-content-xs-center justify-content-sm-center justify-content-lg-end align-items-center ml-lg-50">
          <div class="col-xs-12 col-sm-9 col-md border rounded py-10 px-2">
            <div class="d-flex justify-content-center">
              <ion-icon class="fs-37" name="mail-outline" style="margin-top: 0px" />
            </div>
            <p class="fs-13 col-11 mt-1 mb-10 text-center line-height-p-mulher px-0 mx-auto">
              Mande um e-mail para a Grazi
            </p>
            <div class="d-flex pt-1 justify-content-center">
              <a href="mailto:" class="text-center btn btn-outline-light border-radius-0 btn-sm">
                Envie seu email <i class="fab fa-telegram-plane ml-1 mb-1" />
              </a>
            </div>
          </div>
          <div class="col-xs-12 col-sm-9 col-md border rounded py-10 my-xs-20 my-sm-20 my-md-0 mx-md-40 mx-lg-10 mx-xl-20 px-0">
            <div class="d-flex justify-content-center">
              <ion-icon class="fs-37" name="call-outline" style="margin-top: 0px" />
            </div>
            <p class="fs-13 col-11 mt-1 mb-10 text-center line-height-p-mulher mx-auto px-0">
              Ligue diretamente para a Grazi
            </p>
            <div class="d-flex pt-1 justify-content-center">
              <a href="mailto:" class="text-center btn btn-outline-light border-radius-0 btn-sm">
                Ligue agora <i class="fa fa-phone-alt fs-12 ml-1 mb-1" />
              </a>
            </div>
          </div>
          <div class="col-xs-12 col-sm-9 col-md border rounded py-10 px-2">
            <div class="d-flex justify-content-center">
              <ion-icon class="fs-37" name="reader-outline" style="margin-top: 0px" />
            </div>
            <p class="fs-13 col-11 mt-1 mb-10 text-center line-height-p-mulher px-0 mx-auto">
              Preencha nosso formulário
            </p>
            <div class="d-flex pt-1 justify-content-center">
              <a href="mailto:" class="text-center btn btn-outline-light border-radius-0 btn-sm">
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
      default: 'Agência de Detetives particulares Graziela Bastos'
    },
    descriptionHome: {
      type: String,
      default:
      `A Agência de detetives particulares Graziela Bastos está a mais de 24 anos no mercado
      proporcionando para seus clientes investigações de qualidade além de segurança e confidenciabilidade. 
      omos peritos em investigação conjugal, investigação empresarial, localização de pessoas desaparecidas,
      software espião para filhos menores e muitos outros serviços.
      `
    },
    nameBtnHomeServicos: {
      type: String,
      default: 'Nossos serviços'
    },
    nameBtnHomeContact: {
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
    bgSoftware: {
      type: Boolean,
      default: false
    },
    bgProvas: {
      type: Boolean,
      default: false
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
    background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/bg-home.webp) center center no-repeat;
    -o-background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/bg-home.webp) center center no-repeat;
    -moz-background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/bg-home.webp) center center no-repeat;
    -webkit-background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/bg-home.webp) center center no-repeat;
    background-size: cover;
  }
  .bg-investigacao-empresarial{
    background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/bg-home.webp) center center no-repeat;
    -o-background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/bg-home.webp) center center no-repeat;
    -moz-background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/bg-home.webp) center center no-repeat;
    -webkit-background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/bg-home.webp) center center no-repeat;
    background-size: cover;
  }
  .bg-investigacao-politica{
    background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/bg-home.webp) center center no-repeat;
    -o-background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/bg-home.webp) center center no-repeat;
    -moz-background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/bg-home.webp) center center no-repeat;
    -webkit-background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/bg-home.webp) center center no-repeat;
    background-size: cover;
  }
  .bg-localizacao-de-pessoas{
    background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/bg-home.webp) center center no-repeat;
    -o-background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/bg-home.webp) center center no-repeat;
    -moz-background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/bg-home.webp) center center no-repeat;
    -webkit-background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/bg-home.webp) center center no-repeat;
    background-size: cover;
  }
  .separation-home{
    position: absolute;
    height: 4px;
    width: 300px;
    bottom: -20px;
    border-radius: 3px;
    background-color: var(--roxo);
  }
  .traco-mulher{
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 84%;
    z-index: 0;
  }
  @media (min-width: 992px) {
    .float-lg-left{
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
    background-color: var(--roxo);
  }
</style>
