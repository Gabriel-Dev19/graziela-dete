<template>
  <div>
    <div class="bg-motivos mt-100">
      <div class="container">
        <h1 class="font-teko text-white position-relative col-12 px-0 d-flex justify-content-center text-uppercase text-center">
          Porquê a Agência Graziella Bastos?
          <div class="separation-tema" />
        </h1>
        <p class="col-xl-10 mx-auto text-center text-white mt-4">
          Conduzimos investigações de forma detalhada e completa, todas as provas coletadas
          são de extrema confidenciabilidade e entregues somente ao cliente. Além disso
          todas as nossas investigações são conduzidas de forma totalmente discreta e disfarçada,
          tudo para que o sigilo seja preservado.
        </p>
        <div class="d-flex mt-40 justify-content-center">
          <ion-icon class="text-white fs-60" name="chevron-down-circle-outline" style="--ionicon-stroke-width: 15px;" />
        </div>
      </div>
    </div>
    <div class="container d-flex justify-content-center row mx-auto container-conteudo-motivos">
      <div class="col-sm-10 col-md col-lg-5 col-xl-4 bg-paper py-60 shadow-sm border">
        <div class="col-xs-7 col-sm-7 col-lg-6 d-flex justify-content-center mx-auto px-2">
          <div>
            <img src="../assets/img/agencia-preparada.webp" class="img-fluid rounded-circle shadow" alt="">
          </div>
        </div>
        <h2 class="font-teko text-center mb-1 text-uppercase mt-30">
          Agência preparada
        </h2>
        <p class="fw-500 col-11 mb-0 px-0 mx-auto text-center">
          Trabalhando com uma agência de investigação você não corre
          riscos de chantagens e extorção de enganadores.
        </p>
      </div>
      <div class="col-sm-10 col-md col-lg-5 col-xl-4 mt-xs-30 mt-sm-30 mt-md-0 ml-md-50 bg-paper py-60 shadow-sm border">
        <div class="col-xs-7 col-sm-7 col-lg-6 d-flex justify-content-center mx-auto px-2">
          <div>
            <img src="../assets/img/profissionais-capacitados.webp" class="img-fluid rounded-circle shadow" alt="">
          </div>
        </div>
        <h2 class="font-teko text-center mb-1 text-uppercase mt-30">
          Grandes detetives
        </h2>
        <p class="fw-500 col-11 mb-0 px-0 mx-auto text-center">
          A Agência de detetives Graziella Bastos só trabalha com
          profissionais altamente capacitados e discretos.
        </p>
      </div>
    </div>
  </div>
</template>
<script>
export default {

}
</script>
<style scoped>
  .bg-motivos{
    background: linear-gradient(#000000a6, #000000a6), url(../assets/img/interrogatorio.webp) top center no-repeat;
    background: -o-linear-gradient(#000000a6, #000000a6), url(../assets/img/interrogatorio.webp) top center no-repeat;
    background: -moz-linear-gradient(#000000a6, #000000a6), url(../assets/img/interrogatorio.webp) top center no-repeat;
    background: -webkit-linear-gradient(#000000a6, #000000a6), url(../assets/img/interrogatorio.webp) top center no-repeat;
    background-size: cover;
    padding-top: 100px;
    padding-bottom: 300px;
  }
  .bg-paper{
    background: url(../assets/img/bg-paper.webp) center center no-repeat;
    background-size: cover;
  }
  .separation-tema{
    position: absolute;
    height: 3px;
    width: 150px;
    bottom: -10px;
    border-radius: 3px;
    background-color: var(--roxo);
  }
  img{
    border: 2px solid var(--roxo);
  }
  .container-conteudo-motivos{
    margin-top: -235px;
  }
</style>
