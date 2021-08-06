<template>
  <div class="pt-120">
    <div class="container px-0 position-relative d-flex justify-content-center row mx-auto pb-80">
      <b-carousel
        id="carousel-comentarios"
        ref="carouselComentarios"
        :interval="7000"
        class="mx-auto mx-0 col-12"
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
          <p class="fw-500 text-center mt-10 col-lg-10 px-xs-0 mx-auto">
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
          <p class="fw-500 text-center mt-10 col-lg-10 px-xs-0 mx-auto">
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
          <p class="fw-500 text-center mt-10 col-lg-10 px-xs-0 mx-auto">
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
          <p class="fw-500 text-center mt-10 col-lg-10 px-xs-0 mx-auto">
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
  </div>
</template>
<script>
export default {
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
  .div-indicadores{
    position: absolute;
    bottom: 0px;
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
