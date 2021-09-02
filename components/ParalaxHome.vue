<template>
  <div class="bg-paralaxx pb-70">
    <div class="container">
      <h1 class="font-teko text-white position-relative col-12 px-0 d-flex justify-content-center text-uppercase text-center">
        O que pode esperar de nós?
        <div class="separation-tema" />
      </h1>
      <p class="col-xl-10 mx-auto text-center text-white mt-4">
        Conduzimos investigações de forma detalhada e completa, todas as provas coletadas
        são de extrema confidenciabilidade e entregues somente ao cliente.
      </p>
      <div class="d-flex row mx-auto">
        <div class="col-lg bg-white-50 mt-40 py-50">
          <div class="d-flex justify-content-center">
            <div class="position-relative px-10 py-10">
              <div class="quadrado-alvo-1" />
              <div class="quadrado-alvo-2" />
              <div class="quadrado-alvo-3" />
              <div class="quadrado-alvo-4" />
              <ion-icon class="fs-70" name="alert-circle-outline" style="margin-bottom: -7px; --ionicon-stroke-width: 23px;" />
            </div>
          </div>
          <h5 class="fw-600 col-11 px-0 mx-auto mt-25 fs-17 mb-0 text-center">
            <span class="fw-700">Discrição e sigilo:</span> Peça um orçamento grátis. Garantimos discrição e a sua confidencialidade.
          </h5>
          <div class="d-flex justify-content-center mt-20">
            <btn-roxo-contato-scroll name-btn="Contate um detetive" />
          </div>
        </div>
        <div class="col-lg bg-white-50 mt-40 mx-lg-50 py-50">
          <div class="d-flex justify-content-center">
            <div class="position-relative px-10 py-10">
              <div class="quadrado-alvo-1" />
              <div class="quadrado-alvo-2" />
              <div class="quadrado-alvo-3" />
              <div class="quadrado-alvo-4" />
              <ion-icon class="fs-70" name="receipt-outline" style="margin-bottom: -7px; --ionicon-stroke-width: 23px;" />
            </div>
          </div>
          <h5 class="fw-600 col-11 px-0 mx-auto mt-25 fs-17 mb-0 text-center">
            <span class="fw-700">Relatórios detalhados:</span> Com dados específicos e comprovados que podem ser usados legalmente.
          </h5>
          <div class="d-flex justify-content-center mt-20">
            <btn-roxo-contato-scroll name-btn="Precisa de provas ?" />
          </div>
        </div>
        <div class="col-lg bg-white-50 mt-40 py-50">
          <div class="d-flex justify-content-center">
            <div class="position-relative px-10 py-10">
              <div class="quadrado-alvo-1" />
              <div class="quadrado-alvo-2" />
              <div class="quadrado-alvo-3" />
              <div class="quadrado-alvo-4" />
              <ion-icon class="fs-70" name="time-outline" style="margin-bottom: -7px; --ionicon-stroke-width: 23px;" />
            </div>
          </div>
          <h5 class="fw-600 col-11 px-0 mx-auto mt-25 fs-17 mb-0 text-center">
            <span class="fw-700">24H, 7 dias da semana:</span> Contate-nos agora, não espere por amanhã. Podemos aliviar a sua preocupação hoje mesmo.
          </h5>
          <div class="d-flex justify-content-center mt-20">
            <btn-roxo-contato-scroll name-btn="Monitore tudo!" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import BtnRoxoContatoScroll from './buttons/BtnRoxoContatoScroll.vue'
export default {
  components: { BtnRoxoContatoScroll }

}
</script>
<style scoped>
  .bg-paralaxx{
    background: linear-gradient(#000000a6, #000000a6), url(../assets/img/paralax-home.webp) top center no-repeat;
    background: -o-linear-gradient(#000000a6, #000000a6), url(../assets/img/paralax-home.webp) top center no-repeat;
    background: -moz-linear-gradient(#000000a6, #000000a6), url(../assets/img/paralax-home.webp) top center no-repeat;
    background: -webkit-linear-gradient(#000000a6, #000000a6), url(../assets/img/paralax-home.webp) top center no-repeat;
    background-size: cover;
    padding-top: 100px;
  }
  .separation-tema{
    position: absolute;
    height: 3px;
    width: 150px;
    bottom: -10px;
    border-radius: 3px;
    background-color: var(--roxo_escuro);
  }
  .quadrado-alvo-1{
    position: absolute;
    top: 0;
    left: 0;
    width: 20px;
    height: 20px;
    border-top: 2px solid var(--roxo_escuro);
    border-left: 2px solid var(--roxo_escuro);
  }
  .quadrado-alvo-2{
    position: absolute;
    top: 0;
    right: 0;
    width: 20px;
    height: 20px;
    border-top: 2px solid var(--roxo_escuro);
    border-right: 2px solid var(--roxo_escuro);
  }
  .quadrado-alvo-3{
    position: absolute;
    bottom: 0;
    left: 0;
    width: 20px;
    height: 20px;
    border-bottom: 2px solid var(--roxo_escuro);
    border-left: 2px solid var(--roxo_escuro);
  }
  .quadrado-alvo-4{
    position: absolute;
    bottom: 0;
    right: 0;
    width: 20px;
    height: 20px;
    border-bottom: 2px solid var(--roxo_escuro);
    border-right: 2px solid var(--roxo_escuro);
  }
  .fs-70{
    font-size: 70px;
  }
  .bg-white-50{
    background-color: #ffffffb8;
  }
</style>
