<template scoped>
  <div>
    <div id="content-servicos-1" v-scroll="ScrollContent" class="col-md-10 col-lg-12 px-0 d-flex position-relative justify-content-end align-items-center row mx-auto">
      <div :class="{'show-content-servicos-1': ShowContentScroll}" class="conteudo-left hide-content-servicos-1 shadow pb-xs-20 pb-sm-20 pt-xs-40 pt-sm-40 py-lg-20 order-xs-2 order-sm-2 order-lg-1 col-lg-6 px-lg-20">
        <h1 class="font-teko mb-1 text-white text-xs-center text-sm-center fw-400 text-lg-left text-uppercase">
          Investigação conjugal
        </h1>
        <h5 class="text-uppercase d-flex justify-content-xs-center justify-content-sm-center justify-content-lg-start position-relative text-white-50 font-teko">
          Serviços de detetive
          <div class="borda-tema-servicos" />
        </h5>
        <p class="text-white text-xs-center text-lg-left text-sm-center mt-4">
          Tem dúvidas quanto ao seu companheiro(a)? Não se iniba de saber a verdade! Temos a opção certa para resolver o seu problema!
          Muitas vezes em relacionamentos, há a necessidade de reafirmar a sua fidelidade, ou, quando surge a
          suspeita de adultério, é possível contratar um serviço especializado de investigação conjugal.
        </p>
        <div class="d-flex justify-content-xs-center justify-content-sm-center justify-content-lg-start position-relative align-items-center">
          <h1 class="text-white font-teko fs-45 fw-400">
            1448
          </h1>
          <div class="borda-numeros mb-3 mx-10" />
          <h3 class="text-white mb-10 font-teko text-uppercase">
            Experiências
          </h3>
          <div class="borda-numeros-servicos" />
        </div>
        <div class="d-flex mt-3 justify-content-xs-center justify-content-sm-center justify-content-lg-start">
          <BtnLightTekoRouter router-to="/servicos/investigacao-conjugal/" />
          <BtnLightTekoWhatsApp class="ml-3" />
        </div>
      </div>
      <div :class="{'show-img-servicos-1': ShowImgScroll}" class="col-lg-7 hide-img-servicos-1 px-0">
        <img src="../../assets/img/servicos/bg-conjugal.webp" class="img-fluid shadow" alt="Investigação conjugal">
      </div>
    </div>
    <div class="bb-roxo col-md-10 col-lg-12 mx-auto d-flex justify-content-center align-items-center col-12 my-xs-60 my-sm-70 my-lg-110 my-xl-80">
      <div class="seta-borda px-25">
        <ion-icon class="fs-35 text-roxo-escuro mt-2" name="chevron-down-circle-outline" style="--ionicon-stroke-width: 14px;" />
      </div>
    </div>
  </div>
</template>
<script>
import BtnLightTekoRouter from '../buttons/BtnLightTekoRouter.vue'
import BtnLightTekoWhatsApp from '../buttons/BtnLightTekoWhatsApp.vue'
export default {
  components: {
    BtnLightTekoWhatsApp,
    BtnLightTekoRouter
  },
  data () {
    return {
      ShowContentScroll: true,
      ShowImgScroll: true
    }
  },
  mounted () {
    this.ShowContentScroll = false
    this.ShowImgScroll = false
  },
  methods: {
    ScrollContent () {
      const Janela = document.body.getBoundingClientRect()
      const ContainerScroll = document.getElementById('content-servicos-1').getBoundingClientRect()
      const OffsetScroll = ContainerScroll.top - Janela.top
      if (window.scrollY > OffsetScroll - window.innerHeight + 50) {
        this.ShowContentScroll = true
        this.ShowImgScroll = true
      } else {
        this.ShowContentScroll = false
        this.ShowImgScroll = false
      }
    }
  }
}
</script>
<style scoped>
  .hide-content-servicos-1{
    transform: translateX(-100px);
    -o-transform: translateX(-100px);
    -moz-transform: translateX(-100px);
    -webkit-transform: translateX(-100px);
    opacity: 0;
    transition: all .5s;
    -o-transition: all .5s;
    -moz-transition: all .5s;
    -webkit-transition: all .5s;
  }
  .hide-img-servicos-1{
    transform: translateX(100px);
    -o-transform: translateX(100px);
    -moz-transform: translateX(100px);
    -webkit-transform: translateX(100px);
    opacity: 0;
    transition: all .5s;
    -o-transition: all .5s;
    -moz-transition: all .5s;
    -webkit-transition: all .5s;
  }
  .show-content-servicos-1{
    transform: translateX(0px) !important;
    -o-transform: translateX(0px) !important;
    -moz-transform: translateX(0px) !important;
    -webkit-transform: translateX(0px) !important;
    opacity: 1 !important;
    transition: all .5s;
    -o-transition: all .5s;
    -moz-transition: all .5s;
    -webkit-transition: all .5s;
  }
  .show-img-servicos-1{
    transform: translateX(0px) !important;
    -o-transform: translateX(0px) !important;
    -moz-transform: translateX(0px) !important;
    -webkit-transform: translateX(0px) !important;
    opacity: 1 !important;
    transition: all .5s;
    -o-transition: all .5s;
    -moz-transition: all .5s;
    -webkit-transition: all .5s;
  }
  .separation-tema{
    position: absolute;
    height: 3px;
    width: 80px;
    bottom: -10px;
    border-radius: 3px;
    background-color: var(--roxo_escuro);
  }
  .borda-tema-servicos{
    position: absolute;
    height: 1px;
    width: 250px;
    bottom: -10px;
    border-radius: 3px;
    background-color: var(--white);
  }
  .borda-numeros-servicos{
    position: absolute;
    height: 1px;
    width: 250px;
    bottom: 6px;
    border-radius: 3px;
    background-color: var(--white);
  }
  .borda-numeros{
    height: 3px;
    width: 10px;
    border-radius: 3px;
    background-color: var(--white);
  }
  .conteudo-left{
    background-color: var(--roxo_escuro);
  }
  .conteudo-right{
    background-color: var(--roxo_escuro);
  }
  @media (min-width: 992px) {
    .conteudo-left{
      position: absolute;
      left: 0;
      z-index: 1;
    }
    .conteudo-right{
      position: absolute;
      right: 0;
      z-index: 1;
    }
  }
  .bb-roxo{
    border-bottom: 1px solid var(--roxo_escuro);
  }
  .seta-borda{
    position: absolute;
    background-color: var(--light);
  }
  @media (min-width: 1px) {
    .height-div-servicos{
      min-height: 250px;
    }
  }
  @media (min-width: 992px) {
    .height-div-servicos{
      min-height: 350px;
    }
  }
  h1.font-teko{
    line-height: 38px;
    letter-spacing: 1px;
  }
  h5.font-teko{
    line-height: 15px;
    letter-spacing: 1px;
  }
</style>
