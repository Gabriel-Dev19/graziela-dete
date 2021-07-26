<template>
  <div class="py-xs-50 py-sm-90 d-flex align-items-center bg-home">
    <div class="container mt-110">
      <h1 class="text-white text-center position-relative d-flex px-0 justify-content-center col-xl-8 mx-auto text-uppercase fw-400 display-sm-4 display-lg-3 font-teko">
        {{ titleHome }}
        <div class="separation-home" />
      </h1>
      <p class="text-white text-center col-xl-10 px-0 mx-auto mt-45">
        {{ descriptionHome }}
      </p>
      <div class="d-flex mt-4 justify-content-center">
        <a :href="hashBtn" class="btn btn-lg btn-roxo px-30 fs-18">
          {{ nameBtnHome }}
        </a>
      </div>
      <div class="d-flex mt-70 align-items-center">
        <div class="col separation-redes-home mr-3" />
        <div class="d-flex">
          <a href="http://" target="_blank" rel="noopener noreferrer">
            <i class="fab fs-22 text-roxo fa-twitter" />
          </a>
          <a href="http://" target="_blank" class="mx-15" rel="noopener noreferrer">
            <i class="fab fs-22 text-roxo fa-facebook" />
          </a>
          <a href="http://" target="_blank" rel="noopener noreferrer">
            <i class="fab fs-22 text-roxo fa-youtube" />
          </a>
          <a href="http://" target="_blank" class="mx-15" rel="noopener noreferrer">
            <i class="fab fs-22 text-roxo fa-pinterest" />
          </a>
          <a href="http://" target="_blank" rel="noopener noreferrer">
            <i class="fab fs-22 text-roxo fa-instagram" />
          </a>
        </div>
        <div class="col separation-redes-home ml-3" />
      </div>
    </div>
  </div>
</template>
<script>
export default {
  props: {
    titleHome: {
      type: String,
      default: 'Agência de Detetives particulares Graziela Bastos'
    },
    descriptionHome: {
      type: String,
      default: 'A Agência de detetives particulares Graziela Bastos está a mais de 24 anos no mercado proporcionando para seus clientes investigações de qualidade além de segurança e confidenciabilidade. Somos peritos em investigação conjugal, investigação empresarial, localização de pessoas desaparecidas, software espião para filhos menores e muitos outros serviços'
    },
    nameBtnHome: {
      type: String,
      default: 'Nossos serviços'
    },
    hashBtn: {
      type: String,
      default: '#servicos'
    }
  }
}
</script>
<style scoped>
  .bg-home{
    background: linear-gradient(90deg, #000000c4, #000000c4), url(../assets/img/bg-home.webp) center center no-repeat;
    background-size: cover;
  }
  .separation-home{
    position: absolute;
    height: 4px;
    width: 300px;
    bottom: -20px;
    border-radius: 3px;
    background-color: var(--roxo);
  }
  .separation-redes-home{
    height: 2px;
    border-radius: 3px;
    background-color: var(--roxo);
  }
</style>
