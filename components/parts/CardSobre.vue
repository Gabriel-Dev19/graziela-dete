<template>
  <b-carousel
    id="carousel-sobre"
    indicators
    :interval="5000"
  >
    <b-carousel-slide>
      <div class="bg-roxo-escuro pt-3 pl-3 pr-3 pb-45">
        <img src="../../assets/img/servicos/bg-conjugal.webp" class="img-fluid" alt="Investigação conjugal">
        <h3 class="font-teko text-uppercase mt-4 mb-1 text-center text-white">
          Investigação conjugal
        </h3>
        <p class="text-center fs-14 text-white">
          Tem dúvidas quanto ao seu companheiro(a)? Não se iniba de saber a verdade!
          Temos a opção certa para resolver o seu problema!
        </p>
        <div class="d-flex justify-content-center">
          <BtnLightTekoRouter name-btn="Investigação conjugal" router-to="/servicos/investigacao-conjugal/" />
        </div>
      </div>
    </b-carousel-slide>
    <b-carousel-slide>
      <div class="bg-roxo-escuro pt-3 pl-3 pr-3 pb-45">
        <img src="../../assets/img/servicos/bg-empresarial.webp" class="img-fluid" alt="Investigação empresarial">
        <h3 class="font-teko text-uppercase mt-4 mb-1 text-center text-white">
          Investigação empresarial
        </h3>
        <p class="text-center fs-14 text-white">
          Se você necessita dos serviços de Investigação Empresarial, saiba que a
          Agência de Detetives Graziella Bastos atua no ramo há 15 anos
        </p>
        <div class="d-flex justify-content-center">
          <BtnLightTekoRouter name-btn="Investigação empresarial" router-to="/servicos/investigacao-empresarial/" />
        </div>
      </div>
    </b-carousel-slide>
    <b-carousel-slide>
      <div class="bg-roxo-escuro pt-3 pl-3 pr-3 pb-45">
        <img src="../../assets/img/servicos/bg-software.webp" class="img-fluid" alt="Celular VIP de celular para filhos menores">
        <h3 class="font-teko text-uppercase mt-4 mb-1 text-center text-white">
          Celular VIP
        </h3>
        <p class="text-center fs-14 text-white">
          Obtenha acesso remoto a todas as atividades do celular do seu filho.
          Todas as informações são armazenadas de modo seguro e protegido
        </p>
        <div class="d-flex justify-content-center">
          <BtnLightTekoRouter name-btn="Celular VIP" router-to="/servicos/celular-VIP/" />
        </div>
      </div>
    </b-carousel-slide>
  </b-carousel>
</template>
<script>
import BtnLightTekoRouter from '../buttons/BtnLightTekoRouter.vue'
export default {
  components: {
    BtnLightTekoRouter
  }
}
</script>
