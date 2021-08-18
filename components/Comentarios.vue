<template>
  <div class="pt-130">
    <div class="container px-0 position-relative d-flex justify-content-center row mx-auto pb-80">
      <h1 class="font-teko position-relative col-12 d-flex justify-content-center text-uppercase text-center">
        Nosso trabalho fala por sí!
        <div class="separation-tema" />
      </h1>
      <b-carousel
        id="carousel-comentarios"
        ref="carouselComentarios"
        :interval="7000"
        class="mx-auto mx-0 mt-60 col-12"
        @sliding-start="VerificaSlide"
      >
        <b-carousel-slide>
          <div>
            <div class="d-flex justify-content-center">
              <div class="profile-principal mx-auto d-flex justify-content-center align-items-center">
                <i class="fa fa-user fw-300 fs-50 text-roxo-escuro" />
              </div>
            </div>
            <h5 class="text-center mt-20 fw-700">
              Juliana Santos / Floarianópolis - SC
            </h5>
          </div>
          <p class="fw-500 text-center mt-10 col-lg-10 fs-17 px-xs-0 mx-auto">
            <i class="fas fa-quote-left text-roxo" /> Lorem ipsum dolor, sit amet consectetur adipisicing elit. Ullam, numquam ad temporibus cumque accusantium
            assumenda quibusdam officiis iste ex optio rem vel soluta placeat enim, atque minima
            porro voluptas consectetur
            placeat enim, atque minima
            porro voluptas consectetur
            <i class="fas fa-quote-right text-roxo" />
          </p>
        </b-carousel-slide>
        <b-carousel-slide>
          <div>
            <div class="d-flex justify-content-center">
              <div class="profile-principal mx-auto d-flex justify-content-center align-items-center">
                <i class="fa fa-user fw-300 fs-50 text-roxo-escuro" />
              </div>
            </div>
            <h5 class="text-center mt-20 fw-700">
              Fabrício Cavalcante / Mafra - SC
            </h5>
          </div>
          <p class="fw-500 text-center mt-10 col-lg-10 fs-17 px-xs-0 mx-auto">
            <i class="fas fa-quote-left text-roxo" /> Lorem ipsum dolor, sit amet consectetur adipisicing elit. Ullam, numquam ad temporibus cumque accusantium
            assumenda quibusdam officiis iste ex optio rem vel soluta placeat enim, atque minima
            porro voluptas consectetur
            placeat enim, atque minima
            porro voluptas consectetur
            <i class="fas fa-quote-right text-roxo" />
          </p>
        </b-carousel-slide>
        <b-carousel-slide>
          <div>
            <div class="d-flex justify-content-center">
              <div class="profile-principal mx-auto d-flex justify-content-center align-items-center">
                <i class="fa fa-user fw-300 fs-50 text-roxo-escuro" />
              </div>
            </div>
            <h5 class="text-center mt-20 fw-700">
              Emmily Fonseca / Blumenal - SC
            </h5>
          </div>
          <p class="fw-500 text-center mt-10 col-lg-10 fs-17 px-xs-0 mx-auto">
            <i class="fas fa-quote-left text-roxo" /> Lorem ipsum dolor, sit amet consectetur adipisicing elit. Ullam, numquam ad temporibus cumque accusantium
            assumenda quibusdam officiis iste ex optio rem vel soluta placeat enim, atque minima
            porro voluptas consectetur
            placeat enim, atque minima
            porro voluptas consectetur
            <i class="fas fa-quote-right text-roxo" />
          </p>
        </b-carousel-slide>
        <b-carousel-slide>
          <div>
            <div class="d-flex justify-content-center">
              <div class="profile-principal mx-auto d-flex justify-content-center align-items-center">
                <i class="fa fa-user fw-300 fs-50 text-roxo-escuro" />
              </div>
            </div>
            <h5 class="text-center mt-20 fw-700">
              Emílio Alencar / Curitiba - PR
            </h5>
          </div>
          <p class="fw-500 text-center mt-10 col-lg-10 fs-17 px-xs-0 mx-auto">
            <i class="fas fa-quote-left text-roxo" /> Lorem ipsum dolor, sit amet consectetur adipisicing elit. Ullam, numquam ad temporibus cumque accusantium
            assumenda quibusdam officiis iste ex optio rem vel soluta placeat enim, atque minima
            porro voluptas consectetur
            placeat enim, atque minima
            porro voluptas consectetur
            <i class="fas fa-quote-right text-roxo" />
          </p>
        </b-carousel-slide>
      </b-carousel>
      <div class="div-indicadores d-flex justify-content-center">
        <div class="indicadores cursor-pointer" :class="{'active': Active1}" @click.prevent="$refs.carouselComentarios.setSlide(0)">
          <div class="profile-comments mx-auto d-flex justify-content-center align-items-center">
            <i class="fa fa-user fw-400 fs-20 text-roxo-escuro" />
          </div>
          <h6 class="text-center mb-0 fs-11 mt-2 fw-600">
            Juliana
          </h6>
        </div>
        <div class="indicadores cursor-pointer mx-20" :class="{'active': Active2}" @click.prevent="$refs.carouselComentarios.setSlide(1)">
          <div class="profile-comments mx-auto d-flex justify-content-center align-items-center">
            <i class="fa fa-user fw-400 fs-20 text-roxo-escuro" />
          </div>
          <h6 class="text-center mb-0 fs-11 mt-2 fw-600">
            Fabrício
          </h6>
        </div>
        <div class="indicadores cursor-pointer" :class="{'active': Active3}" @click.prevent="$refs.carouselComentarios.setSlide(2)">
          <div class="profile-comments mx-auto d-flex justify-content-center align-items-center">
            <i class="fa fa-user fw-400 fs-20 text-roxo-escuro" />
          </div>
          <h6 class="text-center mb-0 fs-11 mt-2 fw-600">
            Emmily
          </h6>
        </div>
        <div class="indicadores cursor-pointer ml-20" :class="{'active': Active4}" @click.prevent="$refs.carouselComentarios.setSlide(3)">
          <div class="profile-comments mx-auto d-flex justify-content-center align-items-center">
            <i class="fa fa-user fw-400 fs-20 text-roxo-escuro" />
          </div>
          <h6 class="text-center mb-0 fs-11 mt-2 fw-600">
            Emílio
          </h6>
        </div>
      </div>
    </div>
    <div class="container d-flex justify-content-center row mx-auto mt-70">
      <div class="col-lg-3 bg-paper shadow-sm border mt-20 py-40">
        <div class="d-flex justify-content-center align-items-end">
          <ion-icon class="text-roxo-escuro fs-29" name="trophy-outline" style="margin-bottom: 5px;" />
          <ion-icon class="text-roxo-escuro fs-70" name="trophy-outline" style="--ionicon-stroke-width: 18px;" />
          <ion-icon class="text-roxo-escuro fs-29" name="trophy-outline" style="margin-bottom: 5px;" />
        </div>
        <h3 class="font-teko text-center mb-0 text-uppercase mt-30">
          Melhor atendimento
        </h3>
        <p class="mb-0 fs-15 text-center">
          Somos preferência no quesito atendimento, pois temos um atendimento personalizado
          para cada necessidade.
        </p>
      </div>
      <div class="col-lg-3 bg-paper shadow-sm border mt-20 mx-lg-4 py-40">
        <div class="d-flex justify-content-center align-items-end">
          <ion-icon class="text-roxo-escuro fs-29" name="medal-outline" style="margin-bottom: 5px;" />
          <ion-icon class="text-roxo-escuro fs-70" name="medal-outline" style="--ionicon-stroke-width: 18px;" />
          <ion-icon class="text-roxo-escuro fs-29" name="medal-outline" style="margin-bottom: 5px;" />
        </div>
        <h3 class="font-teko text-center col-lg-9 col-xl-12 px-0 mx-auto mb-0 text-uppercase mt-30">
          Melhor agência
        </h3>
        <p class="mb-0 fs-15 text-center">
          Nossa agência preza a garantia da investigação, se tornando assim,
          referência quando o assunto é qualidade.
        </p>
      </div>
      <div class="col-lg-3 bg-paper shadow-sm border mt-20 py-40">
        <div class="d-flex justify-content-center align-items-end">
          <ion-icon class="text-roxo-escuro fs-29" name="ribbon-outline" style="margin-bottom: 5px;" />
          <ion-icon class="text-roxo-escuro fs-70" name="ribbon-outline" style="--ionicon-stroke-width: 18px;" />
          <ion-icon class="text-roxo-escuro fs-29" name="ribbon-outline" style="margin-bottom: 5px;" />
        </div>
        <h3 class="font-teko text-center mb-0 text-uppercase mt-30">
          Melhores detetives
        </h3>
        <p class="mb-0 fs-15 text-center">
          Nossa agência conta com um time de detetives extremamente profissionais e dedicados
          com seu trabalho.
        </p>
      </div>
      <h1 class="font-teko position-relative col-12 px-0 mt-70 d-flex justify-content-center text-uppercase text-center">
        Torne-se um detetive de sucesso!
        <div class="separation-tema" />
      </h1>
      <p class="col-lg-10 px-0 text-center mx-auto mb-0 mt-20">
        Você também pode fazer parte da rede de detetives Graziella Bastos! Basta ser maior de idade, ter carteira de motorista,
        possuir um veículo para locomoção e ter certificação em algum curso de detetive particular.
      </p>
      <div class="d-flex row mx-auto col-12 px-0 mt-20 justify-content-center">
        <BtnRoxoContatoScroll class="col-xs-8" name-btn="Trabalhe conosco!" />
        <BtnRoxoFooter class="ml-sm-3 col-xs-8 mt-xs-10" />
      </div>
    </div>
  </div>
</template>
<script>
import BtnRoxoContatoScroll from './buttons/BtnRoxoContatoScroll.vue'
import BtnRoxoFooter from './buttons/BtnRoxoFooter.vue'
export default {
  components: { BtnRoxoContatoScroll, BtnRoxoFooter },
  data () {
    return {
      Active1: true,
      Active2: false,
      Active3: false,
      Active4: false
    }
  },
  methods: {
    VerificaSlide (slide) {
      if (slide === 0) {
        this.Active1 = true
        this.Active2 = false
        this.Active3 = false
        this.Active4 = false
      }
      if (slide === 1) {
        this.Active2 = true
        this.Active1 = false
        this.Active3 = false
        this.Active4 = false
      }
      if (slide === 2) {
        this.Active3 = true
        this.Active1 = false
        this.Active2 = false
        this.Active4 = false
      }
      if (slide === 3) {
        this.Active4 = true
        this.Active1 = false
        this.Active2 = false
        this.Active3 = false
      }
    }
  }
}
</script>
<style scoped>
  .separation-tema{
    position: absolute;
    height: 3px;
    width: 150px;
    bottom: -10px;
    border-radius: 3px;
    background-color: var(--roxo);
  }
  .div-indicadores{
    position: absolute;
    bottom: 0px;
  }
  .fs-70{
    font-size: 70px;
  }
  .bg-paper{
    background: url(../assets/img/bg-paper.webp) center center no-repeat;
    background-size: cover;
  }
  .indicadores{
    opacity: 0.6;
    transition: all .3s;
    -o-transition: all .3s;
    -moz-transition: all .3s;
    -webkit-transition: all .3s;
  }
  .indicadores.active{
    opacity: 1;
  }
  .profile-principal{
    width: 95px;
    height: 95px;
    border-radius: 50%;
    background-color: #a45eea93;
  }
  .profile-comments{
    width: 40px;
    height: 40px;
    border-radius: 50%;
    background-color: #a45eea93;
  }
</style>
