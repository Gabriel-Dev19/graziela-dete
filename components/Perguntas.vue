<template>
  <div class="bg-roxo-escuro position-relative d-flex justify-content-center overflow-hidden pb-40 mt-140">
    <div class="borda-cima" />
    <div class="container">
      <h1 class="font-teko position-relative col-xs-8 mx-auto col-sm-12 d-flex justify-content-center text-uppercase text-center">
        Perguntas frequentes
        <div class="separation-tema" />
      </h1>
      <div class="d-flex row justify-content-between align-items-start mx-auto mt-120">
        <div class="py-2 mt-20 bg-light w-perguntas">
          <button v-b-toggle.perguntas-1 class="btn fw-600 px-15 d-flex text-left justify-content-between align-items-center col-12">
            O que faz um detetive particular? <ion-icon class="text-roxo-escuro col-1 pr-0 fs-23" name="add-circle-outline" />
          </button>
          <b-collapse id="perguntas-1">
            <p class="px-3 pt-10 mb-2">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptas repellendus vero accusantium,
              nisi recusandae hic architecto adipisci deleniti
              voluptatem obcaecati. Facilis suscipit molestias incidunt quisquam cum id culpa architecto quia.
            </p>
          </b-collapse>
        </div>
        <div class="py-2 mt-20 bg-light w-perguntas">
          <button v-b-toggle.perguntas-2 class="btn fw-600 px-15 d-flex text-left justify-content-between align-items-center col-12">
            Como é feita a investigação conjugal? <ion-icon class="text-roxo-escuro col-1 pr-0 fs-23" name="add-circle-outline" />
          </button>
          <b-collapse id="perguntas-2">
            <p class="px-3 pt-10 mb-2">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptas repellendus vero accusantium,
              nisi recusandae hic architecto adipisci deleniti
              voluptatem obcaecati. Facilis suscipit molestias incidunt quisquam cum id culpa architecto quia.
            </p>
          </b-collapse>
        </div>
        <div class="py-2 mt-20 bg-light w-perguntas">
          <button v-b-toggle.perguntas-3 class="btn fw-600 px-15 d-flex text-left justify-content-between align-items-center col-12">
            Como funciona o celular espião? <ion-icon class="text-roxo-escuro col-1 pr-0 fs-23" name="add-circle-outline" />
          </button>
          <b-collapse id="perguntas-3">
            <p class="px-3 pt-10 mb-2">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptas repellendus vero accusantium,
              nisi recusandae hic architecto adipisci deleniti
              voluptatem obcaecati. Facilis suscipit molestias incidunt quisquam cum id culpa architecto quia.
            </p>
          </b-collapse>
        </div>
        <div class="py-2 mt-20 bg-light w-perguntas">
          <button v-b-toggle.perguntas-4 class="btn fw-600 px-15 d-flex text-left justify-content-between align-items-center col-12">
            Quero trabalhar como detetive particuar <ion-icon class="text-roxo-escuro col-1 pr-0 fs-23" name="add-circle-outline" />
          </button>
          <b-collapse id="perguntas-4">
            <p class="px-3 pt-10 mb-2">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptas repellendus vero accusantium,
              nisi recusandae hic architecto adipisci deleniti
              voluptatem obcaecati. Facilis suscipit molestias incidunt quisquam cum id culpa architecto quia.
            </p>
          </b-collapse>
        </div>
        <div class="py-2 mt-20 bg-light w-perguntas">
          <button v-b-toggle.perguntas-5 class="btn fw-600 px-15 d-flex text-left justify-content-between align-items-center col-12">
            Que tipo de informações são coletadas? <ion-icon class="text-roxo-escuro col-1 pr-0 fs-23" name="add-circle-outline" />
          </button>
          <b-collapse id="perguntas-5">
            <p class="px-3 pt-10 mb-2">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptas repellendus vero accusantium,
              nisi recusandae hic architecto adipisci deleniti
              voluptatem obcaecati. Facilis suscipit molestias incidunt quisquam cum id culpa architecto quia.
            </p>
          </b-collapse>
        </div>
        <div class="py-2 mt-20 bg-light w-perguntas">
          <button v-b-toggle.perguntas-6 class="btn fw-600 px-15 d-flex text-left justify-content-between align-items-center col-12">
            O que faz um detetive particular? <ion-icon class="text-roxo-escuro col-1 pr-0 fs-23" name="add-circle-outline" />
          </button>
          <b-collapse id="perguntas-6">
            <p class="px-3 pt-10 mb-2">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptas repellendus vero accusantium,
              nisi recusandae hic architecto adipisci deleniti
              voluptatem obcaecati. Facilis suscipit molestias incidunt quisquam cum id culpa architecto quia.
            </p>
          </b-collapse>
        </div>
        <div class="py-2 mt-20 bg-light w-perguntas">
          <button v-b-toggle.perguntas-7 class="btn fw-600 px-15 d-flex text-left justify-content-between align-items-center col-12">
            Como funciona o celular espião? <ion-icon class="text-roxo-escuro col-1 pr-0 fs-23" name="add-circle-outline" />
          </button>
          <b-collapse id="perguntas-7">
            <p class="px-3 pt-10 mb-2">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptas repellendus vero accusantium,
              nisi recusandae hic architecto adipisci deleniti
              voluptatem obcaecati. Facilis suscipit molestias incidunt quisquam cum id culpa architecto quia.
            </p>
          </b-collapse>
        </div>
        <div class="py-2 mt-20 bg-light w-perguntas">
          <button v-b-toggle.perguntas-8 class="btn fw-600 px-15 d-flex text-left justify-content-between align-items-center col-12">
            Quero trabalhar como detetive particuar <ion-icon class="text-roxo-escuro col-1 pr-0 fs-23" name="add-circle-outline" />
          </button>
          <b-collapse id="perguntas-8">
            <p class="px-3 pt-10 mb-2">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptas repellendus vero accusantium,
              nisi recusandae hic architecto adipisci deleniti
              voluptatem obcaecati. Facilis suscipit molestias incidunt quisquam cum id culpa architecto quia.
            </p>
          </b-collapse>
        </div>
        <div class="d-flex col-12 mt-50 justify-content-center">
          <a class="btn btn-perguntas text-uppercase fs-14 py-10 px-25 border-radius-30 fw-600">
            Faça uma pergunta
          </a>
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
  .bg-perguntas{
    background: linear-gradient(#8854d0a8, #8854d0a8), url(../assets/img/bg-img-perguntas.webp) center center no-repeat;
    background: -o-linear-gradient(#8854d0a8, #8854d0a8), url(../assets/img/bg-img-perguntas.webp) center center no-repeat;
    background: -moz-linear-gradient(#8854d0a8, #8854d0a8), url(../assets/img/bg-img-perguntas.webp) center center no-repeat;
    background: -webkit-linear-gradient(#8854d0a8, #8854d0a8), url(../assets/img/bg-img-perguntas.webp) center center no-repeat;
    background-size: cover;
  }
  .btn-perguntas{
    background-color: #ffffff41;
    color: var(--white);
  }
  .btn-perguntas:hover{
    background-color: var(--white);
    color: var(--grafite);
  }
  @media (min-width: 1px) {
    .borda-cima{
      position: absolute;
      top: -90px;
      background-color: var(--light);
      height: 250px;
      width: 200%;
      z-index: 0;
      border-radius: 50%;
    }
    .w-perguntas{
      width: 100%;
    }
  }
  @media (min-width: 576px) {
    .borda-cima{
      position: absolute;
      top: -145px;
      background-color: var(--light);
      height: 250px;
      width: 130%;
      z-index: 0;
      border-radius: 50%;
    }
  }
  @media (min-width: 992px) {
    .w-perguntas{
      width: 48%;
    }
  }
  .separation-tema{
    position: absolute;
    height: 3px;
    width: 150px;
    bottom: -10px;
    border-radius: 3px;
    background-color: var(--roxo);
  }
</style>
