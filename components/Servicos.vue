<template>
  <div class="overflow-hidden pb-140 mt-120">
    <div class="container d-flex row mx-auto">
      <h1 class="font-teko position-relative col-12 px-0 d-flex justify-content-center text-uppercase text-center">
        Nossos serviços
        <div class="separation-tema" />
      </h1>
      <InvestigacaoConjugal />
      <InvestigacaoEmpresarial />
      <InvestigacaoPolitica />
      <LocalizacaoDePessoas />
      <ProvasParaAdvogados />
      <SoftwareEspiao />
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
