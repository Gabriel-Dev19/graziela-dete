<template>
  <div id="servicos" class="overflow-hidden pb-140 mt-120">
    <div class="container d-flex row mx-auto">
      <h1 class="font-teko position-relative col-12 px-0 d-flex justify-content-center text-uppercase text-center">
        {{ titleServicos }}
        <div class="separation-tema" />
      </h1>
      <div class="mt-70">
        <InvestigacaoConjugal v-show="hideConjugal" />
        <InvestigacaoEmpresarial v-show="hideEmpresarial" />
        <InvestigacaoPolitica v-show="hidePolitica" />
        <LocalizacaoDePessoas v-show="hideLocalizacao" />
        <ProvasParaAdvogados v-show="hideProvas" />
        <SoftwareEspiao v-show="hideSoftware" :hide-seta="hideSetaSoftware" />
      </div>
    </div>
  </div>
</template>
<script>
import InvestigacaoConjugal from './services/InvestigacaoConjugal.vue'
import InvestigacaoEmpresarial from './services/InvestigacaoEmpresarial.vue'
import InvestigacaoPolitica from './services/InvestigacaoPolitica.vue'
import LocalizacaoDePessoas from './services/Localizacao.vue'
import ProvasParaAdvogados from './services/ProvasParaAdvogados.vue'
import SoftwareEspiao from './services/SoftwareEspiao.vue'
export default {
  components: {
    InvestigacaoConjugal,
    InvestigacaoEmpresarial,
    InvestigacaoPolitica,
    LocalizacaoDePessoas,
    ProvasParaAdvogados,
    SoftwareEspiao
  },
  props: {
    titleServicos: {
      type: String,
      default: 'Nossos serviços'
    },
    hideSetaSoftware: {
      type: Boolean,
      default: true
    },
    hideConjugal: {
      type: Boolean,
      default: true
    },
    hideEmpresarial: {
      type: Boolean,
      default: true
    },
    hidePolitica: {
      type: Boolean,
      default: true
    },
    hideLocalizacao: {
      type: Boolean,
      default: true
    },
    hideProvas: {
      type: Boolean,
      default: true
    },
    hideSoftware: {
      type: Boolean,
      default: true
    }
  }
}
</script>
<style scoped>
  .separation-tema{
    position: absolute;
    height: 3px;
    width: 100px;
    bottom: -10px;
    border-radius: 3px;
    background-color: var(--roxo);
  }
</style>
