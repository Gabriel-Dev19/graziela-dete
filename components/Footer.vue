<template>
  <footer class="bg-roxo-escuro pt-70 mt-100">
    <div class="container d-flex row mx-auto">
      <div class="col-xl-4 px-0">
        <h1 class="font-teko mb-1 text-xs-center text-sm-center text-xl-left text-white">
          Graziella Bastos
        </h1>
        <p class="text-white mb-2 text-xs-center text-sm-center text-xl-left fs-14">
          Lorem ipsum dolor sit amet consectetur, adipisicing elit. Modi, eius obcaecati reiciendis nam deserunt, doloribus,
          quia soluta vitae quo ad fuga.
          Modi, eius obcaecati reiciendis nam deserunt, doloribus,
          quia soluta vitae quo ad fuga.
          nam deserunt, doloribus,
          quia soluta vitae quo ad fuga.
        </p>
        <div class="d-flex justify-content-xs-center justify-content-sm-center justify-content-xl-start">
          <button class="font-teko py-0 px-0 text-uppercase d-flex align-items-center fs-20 text-white btn">
            Saiba mais <i class="fa fa-angle-right fw-400 mb-1 ml-1" />
          </button>
        </div>
      </div>
      <div class="borda-separation-footer my-xs-4 my-sm-4 my-xl-0 mx-xl-4" />
      <div class="col-xl-3 d-flex justify-content-center px-0">
        <div class="px-0">
          <h3 class="font-teko mb-1 text-xs-center text-sm-center text-xl-left text-white">
            Links rápidos
          </h3>
          <button class="btn d-block text-xs-center text-sm-center text-xl-left col-12 px-0 py-0 fs-15 text-white btn-link" @click.prevent="$router.push('/servicos/investigacao-conjugal')">
            # Investigação conjugal
          </button>
          <button class="btn d-block text-xs-center text-sm-center text-xl-left col-12 px-0 py-0 fs-15 text-white btn-link" @click.prevent="$router.push('/servicos/investigacao-empresarial')">
            # Investigação empresarial
          </button>
          <button class="btn d-block text-xs-center text-sm-center text-xl-left col-12 px-0 py-0 fs-15 text-white btn-link" @click.prevent="$router.push('/servicos/investigacao-politica')">
            # Investigação política
          </button>
          <button class="btn d-block text-xs-center text-sm-center text-xl-left col-12 px-0 py-0 fs-15 text-white btn-link" @click.prevent="$router.push('/servicos/localizacao-de-pessoas')">
            # Localização de pessoas
          </button>
          <button class="btn d-block text-xs-center text-sm-center text-xl-left col-12 px-0 py-0 fs-15 text-white btn-link" @click.prevent="$router.push('/servicos/provas-para-advogados')">
            # Provas para advogados
          </button>
          <button class="btn d-block text-xs-center text-sm-center text-xl-left col-12 px-0 py-0 fs-15 text-white btn-link" @click.prevent="$router.push('/servicos/software-espiao-de-celular')">
            # Software celular espião (para filhos)
          </button>
          <button class="btn d-block text-xs-center text-sm-center text-xl-left col-12 px-0 py-0 fs-15 text-white btn-link" @click.prevent="$router.push('/politica-de-privacidade')">
            # Políticas de privacidade
          </button>
          <button class="btn d-block text-xs-center text-sm-center text-xl-left col-12 px-0 py-0 fs-15 text-white btn-link" @click.prevent="$router.push('/trabalhe-conosco')">
            # Trabalhe conosco
          </button>
        </div>
      </div>
      <div class="borda-separation-footer my-xs-4 my-sm-4 my-xl-0 mx-xl-4" />
      <div id="footer" class="col-xl px-0" :class="{'animate-footer': PulseAnimate}">
        <h4 class="font-teko mb-1 fs-27 text-xs-center text-sm-center text-xl-left text-white">
          <span class="position-relative mr-2">
            Mulher entende mulher!
            <span class="tarja-branca position-absolute col-12 px-0 text-roxo">
              Mulher entende mulher!
            </span>
          </span>
          <span style="text-decoration: underline;">Canal exclusivo</span> para o
          <span style="text-decoration: underline;">atendimento de mulheres.</span>
        </h4>
        <p class="text-white mt-2 text-xs-center text-sm-center text-xl-left fs-14">
          Se você não se sente a vontade de contar seu caso para um detetive homem, esse canal
          é exclusivo para atendentes mulheres
        </p>
        <div class="col-12 px-xs-0 px-sm-0 px-xl-5 d-flex justify-content-xs-center justify-content-sm-center justify-content-xl-start mt-4">
          <a href="mailto:" class="no-underline">
            <div class="d-flex justify-content-center col-12 px-0">
              <ion-icon class="fs-36 text-white" name="mail-outline" />
            </div>
            <h4 class="text-white text-uppercase font-teko col-12 px-0" style="margin-top: 4px;">
              E-mail
            </h4>
          </a>
          <a href="tel:+55" class="no-underline mx-40">
            <div class="d-flex justify-content-center col-12 px-0">
              <ion-icon class="fs-36 text-white" name="call-outline" />
            </div>
            <h4 class="text-white text-uppercase font-teko col-12 px-0" style="margin-top: 4px;">
              Telefone
            </h4>
          </a>
          <a class="no-underline cursor-pointer" @click.prevent="$root.$emit('ShowModalWhatsapp')">
            <div class="d-flex justify-content-center col-12 px-0">
              <ion-icon class="fs-36 text-white" name="logo-whatsapp" />
            </div>
            <h4 class="text-white text-uppercase font-teko col-12 px-0" style="margin-top: 4px;">
              Mensagem
            </h4>
          </a>
        </div>
      </div>
    </div>
    <div class="bg-roxo-super-escuro py-15 mt-70">
      <div class="container d-flex align-items-center justify-content-xs-center justify-content-sm-center justify-content-lg-between text-white row mx-auto">
        <p class="mb-0 text-xs-center text-sm-center text-lg-left">
          &copy; Copyright - Agência Graziella Bastos - Todos os direitos reservados
        </p>
        <a href="https://wa.me/5588996912604?text=Olá,+Gabriel+gostaria+de+receber+mais+informações+sobre+seu+trabalho+como+programador" target="_blank" class="text-white mt-xs-2 mt-sm-2 mt-lg-0" rel="nopenner noreferrer">
          Desenvolvido por Gabriel Camurça <ion-icon class="fs-20" style="margin-bottom: -5px;" name="logo-vue" />
        </a>
      </div>
    </div>
  </footer>
</template>
<script>
export default {
  data () {
    return {
      PulseAnimate: false
    }
  },
  created () {
    this.$root.$on('PulseFooter', () => {
      setTimeout(() => {
        this.PulseAnimate = true
        setTimeout(() => {
          this.PulseAnimate = false
        }, 1050)
      }, 750)
    })
  }
}
</script>
<style scoped>
  @media (min-width: 1px) {
    .borda-separation-footer{
      width: 100%;
      height: 1px;
      background-color: var(--white);
    }
  }
  @media (min-width: 1200px) {
    .borda-separation-footer{
      width: 1px;
      height: initial;
      background-color: var(--white);
    }
  }
  #icons-cartoes i {
    color: #ffffffd4;
  }
  #icons-cartoes i:hover {
    color: #ffffff;
  }
  footer h4{
    line-height: 28px;
  }
  .icon-card {
    width: 67.5px;
    height: 53px;
    background-color: #ffffffd4;
    margin-top: 3px;
    border-radius: 6px;
  }
  .tarja-branca{
    position: absolute;
    left: 0;
    top: 5px;
    height: 27px;
    padding-left: 3px !important;
    padding-top: 2px;
    background-color: var(--white);
  }
  .icon-card:hover {
    background-color: #ffffff;
  }
  .ml-7-px {
    margin-left: 7px;
  }
  .mr-7-px {
    margin-right: 7.5px;
  }
  .animate-footer{
    animation-name: AnimateFooter;
    animation-duration: 1s;
  }
  @keyframes AnimateFooter {
    from {
      transform: scale3d(1, 1, 1);
      -o-transform: scale3d(1, 1, 1);
      -moz-transform: scale3d(1, 1, 1);
      -webkit-transform: scale3d(1, 1, 1);
      box-shadow: none;
    }
    50% {
      transform: scale3d(1.05, 1.05, 1.05);
      box-shadow: 0 0.5rem 1rem rgba(0, 0, 0, 0.15) !important;
    }
    to {
      transform: scale3d(1, 1, 1);
      -o-transform: scale3d(1, 1, 1);
      -moz-transform: scale3d(1, 1, 1);
      -webkit-transform: scale3d(1, 1, 1);
      box-shadow: none;
    }
  }
  @-o-keyframes AnimateFooter {
    from {
      transform: scale3d(1, 1, 1);
      -o-transform: scale3d(1, 1, 1);
      -moz-transform: scale3d(1, 1, 1);
      -webkit-transform: scale3d(1, 1, 1);
      box-shadow: none;
    }
    50% {
      transform: scale3d(1.05, 1.05, 1.05);
      box-shadow: 0 0.5rem 1rem rgba(0, 0, 0, 0.15) !important;
    }
    to {
      transform: scale3d(1, 1, 1);
      -o-transform: scale3d(1, 1, 1);
      -moz-transform: scale3d(1, 1, 1);
      -webkit-transform: scale3d(1, 1, 1);
      box-shadow: none;
    }
  }
  @-moz-keyframes AnimateFooter {
    from {
      transform: scale3d(1, 1, 1);
      -o-transform: scale3d(1, 1, 1);
      -moz-transform: scale3d(1, 1, 1);
      -webkit-transform: scale3d(1, 1, 1);
      box-shadow: none;
    }
    50% {
      transform: scale3d(1.05, 1.05, 1.05);
      box-shadow: 0 0.5rem 1rem rgba(0, 0, 0, 0.15) !important;
    }
    to {
      transform: scale3d(1, 1, 1);
      -o-transform: scale3d(1, 1, 1);
      -moz-transform: scale3d(1, 1, 1);
      -webkit-transform: scale3d(1, 1, 1);
      box-shadow: none;
    }
  }
  @-webkit-keyframes AnimateFooter {
    from {
      transform: scale3d(1, 1, 1);
      -o-transform: scale3d(1, 1, 1);
      -moz-transform: scale3d(1, 1, 1);
      -webkit-transform: scale3d(1, 1, 1);
      box-shadow: none;
    }
    50% {
      transform: scale3d(1.05, 1.05, 1.05);
      box-shadow: 0 0.5rem 1rem rgba(0, 0, 0, 0.15) !important;
    }
    to {
      transform: scale3d(1, 1, 1);
      -o-transform: scale3d(1, 1, 1);
      -moz-transform: scale3d(1, 1, 1);
      -webkit-transform: scale3d(1, 1, 1);
      box-shadow: none;
    }
  }
</style>
