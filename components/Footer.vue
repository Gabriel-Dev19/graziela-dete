<template>
  <footer class="bg-roxo-escuro pt-70 mt-100">
    <div class="container d-flex row mx-auto">
      <div class="col-lg-4 px-0">
        <h1 class="font-teko mb-1 text-white">
          Graziela Bastos
        </h1>
        <p class="text-white mb-2 fs-14">
          Lorem ipsum dolor sit amet consectetur, adipisicing elit. Modi, eius obcaecati reiciendis nam deserunt, doloribus,
          quia soluta vitae quo ad fuga.
          Modi, eius obcaecati reiciendis nam deserunt, doloribus,
          quia soluta vitae quo ad fuga.
          nam deserunt, doloribus,
          quia soluta vitae quo ad fuga.
        </p>
        <button class="font-teko py-0 px-0 text-uppercase d-flex align-items-center fs-20 text-white btn">
          Saiba mais <i class="fa fa-angle-right fw-400 mb-1 ml-1" />
        </button>
      </div>
      <div class="borda-separation-footer my-xs-4 my-sm-4 my-lg-0 mx-lg-4" />
      <div class="col-lg-3 px-0">
        <h3 class="font-teko mb-1 text-white">
          Links rápidos
        </h3>
        <button class="btn px-0 text-left py-0 fs-15 text-white btn-link">
          # Investigação conjugal
        </button>
        <button class="btn px-0 text-left py-0 fs-15 text-white btn-link">
          # Investigação empresarial
        </button>
        <button class="btn px-0 text-left py-0 fs-15 text-white btn-link">
          # Investigação política
        </button>
        <button class="btn px-0 text-left py-0 fs-15 text-white btn-link">
          # Localização de pessoas
        </button>
        <button class="btn px-0 text-left py-0 fs-15 text-white btn-link">
          # Provas para advogados
        </button>
        <button class="btn px-0 text-left py-0 fs-15 text-white btn-link">
          # Software celular espião (para filhos)
        </button>
        <button class="btn px-0 text-left py-0 fs-15 text-white btn-link">
          # Políticas de provacidade
        </button>
        <button class="btn px-0 text-left py-0 fs-15 text-white btn-link">
          # Trabalhe conosco
        </button>
      </div>
      <div class="borda-separation-footer my-xs-4 my-sm-4 my-lg-0 mx-lg-4" />
      <div class="col-lg px-0">
        <h4 class="font-teko mb-1 fs-27 text-white">
          Mulher entende mulher! <span style="text-decoration: underline;">Canal exclusivo</span> para o
          <span style="text-decoration: underline;">atendimento de mulheres.</span>
        </h4>
        <p class="text-white mt-2 fs-14">
          Se você não se sente a vontade de contar seu caso para um detetive homem, esse canal
          é exclusivo para atendentes mulheres
        </p>
        <div class="col-sm-9 col-md-7 col-lg-12 px-xs-0 px-sm-0 px-xl-5 d-flex mt-4">
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
          <a href="mailto:" class="no-underline">
            <div class="d-flex justify-content-center col-12 px-0">
              <ion-icon class="fs-36 text-white" name="logo-whatsapp" />
            </div>
            <h4 class="text-white text-uppercase font-teko col-12 px-0" style="margin-top: 4px;">
              Whatsapp
            </h4>
          </a>
        </div>
      </div>
    </div>
    <div class="bg-roxo-super-escuro py-15 mt-70">
      <div class="container d-flex align-items-center justify-content-xs-center justify-content-sm-center justify-content-lg-between text-white row mx-auto">
        <p class="mb-0 text-xs-center text-sm-center text-lg-left">
          &copy; Copyright - Agência Graziela Bastos - Todos os direitos reservados
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
  @media (min-width: 992px) {
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
  .icon-card:hover {
    background-color: #ffffff;
  }
  .ml-7-px {
    margin-left: 7px;
  }
  .mr-7-px {
    margin-right: 7.5px;
  }
</style>
