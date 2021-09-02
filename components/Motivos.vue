<template>
  <div>
    <div class="bg-motivos mt-100">
      <div class="container">
        <h1 class="font-teko text-white position-relative col-12 px-0 d-flex justify-content-center text-uppercase text-center">
          Porquê a Agência Graziella Bastos?
          <div class="separation-tema" />
        </h1>
        <p class="col-xl-10 mx-auto text-center text-white mt-4">
          Nosso trabalho é realizado por detetives experientes e devidamente capacitados que trabalham conosco há muitos anos o que garante um trabalho bem executado com rapidez e sigilo absoluto.
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
            <img src="../assets/img/agencia-preparada.webp" class="img-fluid rounded-circle shadow" alt="Agência de detetives detetives investigando um caso">
          </div>
        </div>
        <h2 class="font-teko text-center mb-1 text-uppercase mt-30">
          Garantia de Trabalho
        </h2>
        <p class="fw-500 col-11 mb-0 px-0 mx-auto text-center">
          Garantimos o trabalho realizado através de informações durante o andamento das investigações.
        </p>
      </div>
      <div class="col-sm-10 col-md col-lg-5 col-xl-4 mt-xs-30 mt-sm-30 mt-md-0 ml-md-50 bg-paper py-60 shadow-sm border">
        <div class="col-xs-7 col-sm-7 col-lg-6 d-flex justify-content-center mx-auto px-2">
          <div>
            <img src="../assets/img/profissionais-capacitados.webp" class="img-fluid rounded-circle shadow" alt="Detetives capacitados">
          </div>
        </div>
        <h2 class="font-teko text-center mb-1 text-uppercase mt-30">
          Detetives experientes
        </h2>
        <p class="fw-500 col-11 mb-0 px-0 mx-auto text-center">
          Detetives com anos de experiência em diversos casos para levantar provas e informações.
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
    background-color: var(--roxo_escuro);
  }
  img{
    border: 2px solid var(--roxo_escuro);
  }
  .container-conteudo-motivos{
    margin-top: -235px;
  }
</style>
