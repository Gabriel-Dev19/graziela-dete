<template>
  <div class="pt-100">
    <div class="container">
      <h1 class="font-teko position-relative col-lg-10 mx-auto px-0 d-flex justify-content-center text-uppercase text-center">
        Precisando de um detetive particular em {{ nameCidades }}?
        <div class="separation-tema" />
      </h1>
      <div class="d-flex justify-content-between align-items-start row mx-auto mt-80">
        <div class="col-lg-6 col-xl-7 px-0">
          <h1 class="font-teko d-flex justify-content-xs-center justify-content-sm-center justify-content-lg-start position-relative mb-1">
            Mais informações
            <div class="borda-tema-fina" />
          </h1>
          <p class="mt-3 text-xs-center text-sm-center text-lg-left fw-500 px-0">
            A <b>Agência de Detetives Graziella Bastos</b> está em {{ nameCidades }} e queremos ajudar você a desvendar suas
            dúvidas. Com mais de 15 anos de experiência e muitos casos resolvidos, atuamos em todo o
            território nacional.
          </p>
          <h1 class="font-teko mt-30 d-flex justify-content-xs-center justify-content-sm-center justify-content-lg-start position-relative position-relative mb-1">
            Nossa equipe
            <div class="borda-tema-fina" />
          </h1>
          <p class="mt-3 text-xs-center text-sm-center text-lg-left fw-500 px-0">
            Nossa agência é especializada em investigações de caráter particular, conjugal, empresarial, acompanhamento de
            filhos, localização de bens e pessoas desaparecidas, levantamento de provas para advogados, dentre outras.
            Seja qual for o seu problema e complexidade do caso que você vem enfrentando, a Agência de Detetives
            Graziella Bastos terá a satisfação em ajuda-lo a desvendar.
          </p>
          <div class="d-flex justify-content-xs-center justify-content-sm-center mt-4 justify-content-lg-start">
            <BtnQuatroSete v-show="showQuatroSete" />
            <BtnQuatroOito v-show="showQuatroOito" />
            <BtnQuatroNove v-show="showQuatroNove" />
            <BtnQuatroUm v-show="showQuatroUm" />
            <btn-roxo-contato-scroll v-show="showScroll" name-btn="Contate aqui!" />
          </div>
        </div>
        <div class="col-lg ml-lg-90 mt-xs-70 mt-sm-70 mt-lg-0 px-0">
          <CardSobre />
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import BtnQuatroSete from '../buttons/BtnQuatroSete.vue'
import BtnQuatroOito from '../buttons/BtnQuatroOito.vue'
import BtnQuatroNove from '../buttons/BtnQuatroNove.vue'
import BtnQuatroUm from '../buttons/BtnQuatroUmm.vue'
import BtnRoxoContatoScroll from '../buttons/BtnRoxoContatoScroll.vue'
import CardSobre from './CardSobre.vue'
export default {
  components: { CardSobre, BtnQuatroSete, BtnQuatroOito, BtnQuatroNove, BtnQuatroUm, BtnRoxoContatoScroll },
  props: {
    nameCidades: {
      type: String,
      default: ''
    },
    showQuatroSete: {
      type: Boolean,
      default: false
    },
    showQuatroOito: {
      type: Boolean,
      default: false
    },
    showQuatroNove: {
      type: Boolean,
      default: false
    },
    showQuatroUm: {
      type: Boolean,
      default: false
    },
    showScroll: {
      type: Boolean,
      default: false
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
</style>
