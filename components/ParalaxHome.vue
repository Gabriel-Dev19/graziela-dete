<template>
  <div class="bg-paralaxx mt-130 pb-70">
    <div class="container">
      <h1 class="font-teko text-white position-relative col-12 px-0 d-flex justify-content-center text-uppercase text-center">
        Investigações detalhadas
        <div class="separation-tema" />
      </h1>
      <p class="col-xl-10 mx-auto text-center text-white mt-4">
        Conduzimos investigações de forma detalhada e completa, todas as provas coletadas
        são de extrema confidenciabilidade e entregues somente ao cliente.
      </p>
      <div class="d-flex row mx-auto">
        <div class="col-lg bg-white-50 mt-40 py-50">
          <div class="d-flex justify-content-center">
            <ion-icon class="fs-70" name="receipt-outline" style="--ionicon-stroke-width: 23px;" />
          </div>
          <h5 class="fw-600 col-11 px-0 mx-auto mt-25 fs-17 mb-0 text-center">
            Construímos um dossiê completo com todo o caso documentado
            com todas as provas
          </h5>
          <div class="d-flex justify-content-center mt-20">
            <button class="btn btn-roxo shadow-sm border-radius-0 px-20 fw-500">
              Contate um detetive
            </button>
          </div>
        </div>
        <div class="col-lg bg-white-50 mt-40 mx-lg-50 py-50">
          <div class="d-flex justify-content-center">
            <ion-icon class="fs-70" name="finger-print-outline" style="--ionicon-stroke-width: 10px;" />
          </div>
          <h5 class="fw-600 col-11 px-0 mx-auto mt-25 fs-17 mb-0 text-center">
            Coletamos provas de forma que elas possam ser usadas legalmente
            pela justiça
          </h5>
          <div class="d-flex justify-content-center mt-20">
            <button class="btn btn-roxo shadow-sm border-radius-0 px-20 fw-500">
              Precisa de provas ?
            </button>
          </div>
        </div>
        <div class="col-lg bg-white-50 mt-40 py-50">
          <div class="d-flex justify-content-center">
            <ion-icon class="fs-70" name="footsteps-outline" style="--ionicon-stroke-width: 23px;" />
          </div>
          <h5 class="fw-600 col-11 px-0 mx-auto mt-25 fs-17 mb-0 text-center">
            Fazemos todo o trabalho de campana da pessoa investigada para obeter melhores resultados
          </h5>
          <div class="d-flex justify-content-center mt-20">
            <button class="btn btn-roxo shadow-sm border-radius-0 px-20 fw-500">
              Monitore tudo!
            </button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {

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
    background-color: var(--roxo);
  }
  .fs-70{
    font-size: 70px;
  }
  .bg-white-50{
    background-color: #ffffffb8;
  }
</style>
