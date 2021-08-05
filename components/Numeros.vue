<template>
  <div class="py-100">
    <div class="container d-flex row mx-auto">
      <div class="col-lg-7 px-0">
        <h1 class="font-teko mb-0 text-xs-center text-sm-center text-lg-left text-uppercase">
          Agência Graziela Bastos
        </h1>
        <h5 class="text-uppercase d-flex justify-content-xs-center justify-content-sm-center justify-content-lg-start position-relative fw-600 text-black-50 font-teko">
          Detetives Particulares
          <div class="borda-tema-numeros" />
        </h5>
        <p class="fw-500 text-xs-center text-sm-center text-lg-left mt-25">
          Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quos voluptatibus molestiae fugiat
          eos culpa voluptatum tempora delectus illo dolorum recusandae voluptate, sequi veniam dolor
          dignissimos odit magnam. Ex, quasi similique!
          Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quos voluptatibus molestiae fugiat
          eos culpa voluptatum tempora delectus illo dolorum recusandae voluptate, sequi veniam dolor
          dignissimos odit magnam. Ex, quasi similique!
        </p>
        <h2 class="font-teko text-xs-center text-sm-center text-lg-left mb-0 mt-40 text-uppercase">
          Melhores resultados
        </h2>
        <h6 class="text-uppercase d-flex justify-content-xs-center justify-content-sm-center justify-content-lg-start text-black-50 mb-0 position-relative fs-18 fw-600 font-teko">
          Números surpreendentes
          <div class="borda-tema-numeros" />
        </h6>
        <div class="d-flex justify-content-xs-center justify-content-sm-center justify-content-lg-start row mx-auto">
          <div class="col-xs-6 col-sm-auto mt-20 px-0 py-20">
            <h1 class="font-teko display-4 d-flex justify-content-center position-relative fw-500 text-center">
              128
              <div class="borda-numeros" />
            </h1>
            <h5 class="fw-700 mt-4 text-center text-uppercase fs-14">
              Casos
              <br>
              encerrados
            </h5>
          </div>
          <div class="col-xs-6 col-sm-auto mt-20 px-0 mx-sm-70 py-20">
            <h1 class="font-teko display-4 d-flex justify-content-center position-relative fw-500 text-center">
              109
              <div class="borda-numeros" />
            </h1>
            <h5 class="fw-700 mt-4 text-center text-uppercase fs-14">
              Suspeitas
              <br>
              confirmadas
            </h5>
          </div>
          <div class="col-xs-6 col-sm-auto mt-20 px-0 py-20">
            <h1 class="font-teko display-4 d-flex justify-content-center position-relative fw-500 text-center">
              98
              <div class="borda-numeros" />
            </h1>
            <h5 class="fw-700 mt-4 text-center text-uppercase fs-14">
              Clientes
              <br>
              satisfeitos
            </h5>
          </div>
        </div>
        <div class="d-flex justify-content-xs-center justify-content-sm-center justify-content-lg-start mt-10">
          <button class="btn btn-roxo border-radius-0 px-20">
            Contate um detetive
          </button>
        </div>
      </div>
      <div class="d-xs-none d-sm-none d-lg-block col-lg mt-xs-50 mt-sm-50 mt-lg-0 ml-lg-50 px-0">
        <img src="../assets/img/investigacao-2.webp" class="img-fluid border shadow" alt="">
      </div>
    </div>
  </div>
</template>
<script>
export default {

}
</script>
<style scoped>
  .borda-tema-numeros{
    position: absolute;
    height: 2px;
    width: 250px;
    bottom: -8px;
    border-radius: 3px;
    background-color: var(--roxo);
  }
  .borda-numeros{
    position: absolute;
    height: 3px;
    width: 30px;
    bottom: -11px;
    border-radius: 3px;
    background-color: var(--grafite);
  }
</style>
