<template>
  <div class="pt-70 overflow-hidden pb-140 bg-servicos mt-100">
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
      <software-espiao />
    </div>
  </div>
</template>
<script>
import InvestigacaoConjugal from './services/InvestigacaoConjugal.vue'
import InvestigacaoEmpresarial from './services/InvestigacaoEmpresarial.vue'
import InvestigacaoPolitica from './services/InvestigacaoPolitica.vue'
import LocalizacaoDePessoas from './services/LocalizacaoDePessoas.vue'
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
  #content-servicos-3 {
    transform: translateX(var(--tx_content_3));
    opacity: var(--op_content_3);
    transition: all .4s linear;
    will-change: transform;
  }
  #img-servicos-3 {
    transform: translateX(var(--tx_img_3));
    opacity: var(--op_img_3);
    transition: all .4s linear;
    will-change: transform;
  }
  #content-servicos-4 {
    transform: translateX(var(--tx_content_4));
    opacity: var(--op_content_4);
    transition: all .4s linear;
    will-change: transform;
  }
  #img-servicos-4 {
    transform: translateX(var(--tx_img_4));
    opacity: var(--op_img_4);
    transition: all .4s linear;
    will-change: transform;
  }
  .bg-servicos{
    background-color: #ededed;
  }
</style>
