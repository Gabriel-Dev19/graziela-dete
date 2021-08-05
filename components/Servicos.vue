<template>
  <div class="pt-130">
    <div class="container d-flex row mx-auto">
      <h1 class="font-teko position-relative col-12 px-0 d-flex justify-content-center text-uppercase text-center">
        Nossos serviços
        <div class="separation-tema" />
      </h1>
      <div class="d-flex col-12 mt-50 px-0 row mx-auto">
        <div class="height-div-servicos bg-conjugal d-flex align-items-center shadow col-lg" @mouseenter="$root.$emit('bv::toggle::collapse', 'collapse-conjugal')" @mouseleave="$root.$emit('bv::toggle::collapse', 'collapse-conjugal')">
          <div class="col-12 py-xs-50 py-sm-50">
            <h5 class="text-white-50 font-teko text-uppercase text-center">
              Serviços
            </h5>
            <h2 class="text-white font-teko d-flex justify-content-center position-relative fw-400 mb-0 text-uppercase text-center">
              Investigação conjugal
              <div class="separation-servicos" />
            </h2>
            <b-collapse id="collapse-conjugal">
              <div class="pt-20">
                <p class="text-center text-white mt-2 mb-0 fs-15">
                  Lorem ipsum dolor sit amet, consectetur adipisicing elit. Esse, impedit inventore ex dolores voluptatibus
                  pariatur reprehenderit eos? Molestias inventore tempora reiciendis dolores, est consectetur pariatur.
                  Quidem a ea eum odit?
                </p>
                <div class="d-flex justify-content-center">
                  <button class="btn text-uppercase mt-2 pb-0 px-0 fs-22 d-flex align-items-center fw-500 btn-teko-branco">
                    Saiba mais <i class="fa fa-angle-right fw-400 fs-20 ml-1" style="margin-bottom: 1px" />
                  </button>
                </div>
              </div>
            </b-collapse>
          </div>
        </div>
        <div class="height-div-servicos bg-empresarial d-flex align-items-center mt-xs-20 mt-sm-20 mt-lg-0 ml-lg-20 shadow col-lg" @mouseenter="$root.$emit('bv::toggle::collapse', 'collapse-empresarial')" @mouseleave="$root.$emit('bv::toggle::collapse', 'collapse-empresarial')">
          <div class="col-12 py-xs-50 py-sm-50">
            <h5 class="text-white-50 font-teko text-uppercase text-center">
              Serviços
            </h5>
            <h2 class="text-white font-teko d-flex justify-content-center position-relative fw-400 mb-0 text-uppercase text-center">
              Investigação empresarial
              <div class="separation-servicos" />
            </h2>
            <b-collapse id="collapse-empresarial">
              <div class="pt-20">
                <p class="text-center text-white mt-2 mb-0 fs-15">
                  Lorem ipsum dolor sit amet, consectetur adipisicing elit. Esse, impedit inventore ex dolores voluptatibus
                  pariatur reprehenderit eos? Molestias inventore tempora reiciendis dolores, est consectetur pariatur.
                  Quidem a ea eum odit?
                </p>
                <div class="d-flex justify-content-center">
                  <button class="btn text-uppercase mt-2 pb-0 px-0 fs-22 d-flex align-items-center fw-500 btn-teko-branco">
                    Saiba mais <i class="fa fa-angle-right fw-400 fs-20 ml-1" style="margin-bottom: 1px" />
                  </button>
                </div>
              </div>
            </b-collapse>
          </div>
        </div>
      </div>
      <div class="d-flex col-12 mt-20 px-0 row mx-auto">
        <div class="height-div-servicos bg-politica d-flex align-items-center shadow col-lg-5" @mouseenter="$root.$emit('bv::toggle::collapse', 'collapse-politica')" @mouseleave="$root.$emit('bv::toggle::collapse', 'collapse-politica')">
          <div class="col-12 py-xs-50 py-sm-50">
            <h5 class="text-white-50 font-teko text-uppercase text-center">
              Serviços
            </h5>
            <h2 class="text-white font-teko d-flex justify-content-center position-relative fw-400 mb-0 text-uppercase text-center">
              Investigação política
              <div class="separation-servicos" />
            </h2>
            <b-collapse id="collapse-politica">
              <div class="pt-20">
                <p class="text-center text-white mt-2 mb-0 fs-15">
                  Lorem ipsum dolor sit amet, consectetur adipisicing elit. Esse, impedit inventore ex dolores voluptatibus
                  pariatur reprehenderit eos? Molestias inventore tempora reiciendis dolores, est consectetur pariatur.
                  Quidem a ea eum odit?
                </p>
                <div class="d-flex justify-content-center">
                  <button class="btn text-uppercase mt-2 pb-0 px-0 fs-22 d-flex align-items-center fw-500 btn-teko-branco">
                    Saiba mais <i class="fa fa-angle-right fw-400 fs-20 ml-1" style="margin-bottom: 1px" />
                  </button>
                </div>
              </div>
            </b-collapse>
          </div>
        </div>
        <div class="height-div-servicos bg-localizacao d-flex align-items-center shadow mt-xs-20 mt-sm-20 mt-lg-0 ml-lg-20 col-lg" @mouseenter="$root.$emit('bv::toggle::collapse', 'collapse-localizacao')" @mouseleave="$root.$emit('bv::toggle::collapse', 'collapse-localizacao')">
          <div class="col-12 py-xs-50 py-sm-50">
            <h5 class="text-white-50 font-teko text-uppercase text-center">
              Serviços
            </h5>
            <h2 class="text-white font-teko d-flex justify-content-center position-relative fw-400 mb-0 text-uppercase text-center">
              Localização de pessoas
              <div class="separation-servicos" />
            </h2>
            <b-collapse id="collapse-localizacao">
              <div class="pt-20">
                <p class="text-center text-white mt-2 mb-0 fs-15">
                  Lorem ipsum dolor sit amet, consectetur adipisicing elit. Esse, impedit inventore ex dolores voluptatibus
                  pariatur reprehenderit eos? Molestias inventore tempora reiciendis dolores, est consectetur pariatur.
                  Quidem a ea eum odit?
                </p>
                <div class="d-flex justify-content-center">
                  <button class="btn text-uppercase mt-2 pb-0 px-0 fs-22 d-flex align-items-center fw-500 btn-teko-branco">
                    Saiba mais <i class="fa fa-angle-right fw-400 fs-20 ml-1" style="margin-bottom: 1px" />
                  </button>
                </div>
              </div>
            </b-collapse>
          </div>
        </div>
      </div>
      <div class="d-flex col-12 mt-20 px-0 row mx-auto">
        <div class="height-div-servicos bg-software d-flex align-items-center shadow col-lg" @mouseenter="$root.$emit('bv::toggle::collapse', 'collapse-software')" @mouseleave="$root.$emit('bv::toggle::collapse', 'collapse-software')">
          <div class="col-12 py-xs-50 py-sm-50">
            <h5 class="text-white-50 font-teko text-uppercase text-center">
              Serviços
            </h5>
            <h2 class="text-white font-teko d-flex justify-content-center position-relative fw-400 mb-0 text-uppercase text-center">
              Software espião para filhos menores
              <div class="separation-servicos" />
            </h2>
            <b-collapse id="collapse-software">
              <div class="pt-20">
                <p class="text-center text-white mt-2 mb-0 fs-15">
                  Lorem ipsum dolor sit amet, consectetur adipisicing elit. Esse, impedit inventore ex dolores voluptatibus
                  pariatur reprehenderit eos? Molestias inventore tempora reiciendis dolores, est consectetur pariatur.
                  Quidem a ea eum odit?
                </p>
                <div class="d-flex justify-content-center">
                  <button class="btn text-uppercase mt-2 pb-0 px-0 fs-22 d-flex align-items-center fw-500 btn-teko-branco">
                    Saiba mais <i class="fa fa-angle-right fw-400 fs-20 ml-1" style="margin-bottom: 1px" />
                  </button>
                </div>
              </div>
            </b-collapse>
          </div>
        </div>
        <div class="height-div-servicos bg-provas d-flex align-items-center shadow mt-xs-20 mt-sm-20 mt-lg-0 ml-lg-20 col-lg-5" @mouseenter="$root.$emit('bv::toggle::collapse', 'collapse-provas')" @mouseleave="$root.$emit('bv::toggle::collapse', 'collapse-provas')">
          <div class="col-12 py-xs-50 py-sm-50">
            <h5 class="text-white-50 font-teko text-uppercase text-center">
              Serviços
            </h5>
            <h2 class="text-white font-teko d-flex justify-content-center position-relative fw-400 mb-0 text-uppercase text-center">
              Provas para advogados
              <div class="separation-servicos" />
            </h2>
            <b-collapse id="collapse-provas">
              <div class="pt-20">
                <p class="text-center text-white mt-2 mb-0 fs-15">
                  Lorem ipsum dolor sit amet, consectetur adipisicing elit. Esse, impedit inventore ex dolores voluptatibus
                  pariatur reprehenderit eos? Molestias inventore tempora reiciendis dolores, est consectetur pariatur.
                  Quidem a ea eum odit?
                </p>
                <div class="d-flex justify-content-center">
                  <button class="btn text-uppercase mt-2 pb-0 px-0 fs-22 d-flex align-items-center fw-500 btn-teko-branco">
                    Saiba mais <i class="fa fa-angle-right fw-400 fs-20 ml-1" style="margin-bottom: 1px" />
                  </button>
                </div>
              </div>
            </b-collapse>
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
  .separation-tema{
    position: absolute;
    height: 3px;
    width: 80px;
    bottom: -10px;
    border-radius: 3px;
    background-color: var(--roxo);
  }
  .separation-servicos{
    position: absolute;
    height: 2px;
    width: 80px;
    bottom: -13px;
    border-radius: 3px;
    background-color: var(--roxo);
  }
  @media (min-width: 1px) {
    .height-div-servicos{
      min-height: 250px;
    }
  }
  @media (min-width: 992px) {
    .height-div-servicos{
      min-height: 350px;
    }
  }
  h2.font-teko{
    line-height: 35px;
    letter-spacing: 1px;
  }
  h5.font-teko{
    line-height: 15px;
    letter-spacing: 1px;
  }
  .bg-conjugal{
    background: linear-gradient(#000000b6, #000000b6), url(../assets/img/servicos/bg-conjugal.webp) center center no-repeat;
    background-size: cover;
  }
  .bg-empresarial{
    background: linear-gradient(#000000b6, #000000b6), url(../assets/img/servicos/bg-empresarial.webp) center center no-repeat;
    background-size: cover;
  }
  .bg-politica{
    background: linear-gradient(#000000b6, #000000b6), url(../assets/img/servicos/bg-politica.webp) center center no-repeat;
    background-size: cover;
  }
  .bg-localizacao{
    background: linear-gradient(#000000b6, #000000b6), url(../assets/img/servicos/bg-localizacao.webp) center center no-repeat;
    background-size: cover;
  }
  .bg-provas{
    background: linear-gradient(#000000b6, #000000b6), url(../assets/img/servicos/bg-provas.webp) center center no-repeat;
    background-size: cover;
  }
  .bg-software{
    background: linear-gradient(#000000b6, #000000b6), url(../assets/img/servicos/bg-software.webp) center center no-repeat;
    background-size: cover;
  }
</style>
