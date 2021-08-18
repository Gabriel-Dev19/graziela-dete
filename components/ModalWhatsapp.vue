<template>
  <div>
    <b-modal
      id="modal-whatsapp"
      hide-footer
      hide-header
      centered
      size="xl"
      class="borda px-0"
    >
      <div>
        <div class="py-15 px-3 position-relative bg-roxo-escuro">
          <h2 class="text-white col-xs-10 mx-auto text-center mb-0 font-teko text-uppercase">
            Central de atendimento
          </h2>
          <p class="text-white text-center fs-xs-15 col-lg-8 px-0 mx-auto mb-0">
            Contate um de nossos especialistas na sua região, ou em uma região próxima, explique seu caso,
            com certeza será um prazer lhe ajudar!
          </p>
          <button class="btn btn-fechar-modal" @click.prevent="$bvModal.hide('modal-whatsapp')">
            <i class="fa fa-times" />
          </button>
        </div>
        <div class="pt-20 pb-50 col-12 px-lg-50 px-xl-70 d-flex row mx-auto bg-light">
          <a href="https://wa.me/5547991062096?text=Olá,+estou+visitando+o+site+da+Gaziella+Bastos+e+gostaria+de+receber+mais+informações" target="_blank" class="row mx-0 col-lg-6 col-xl-4 no-underline d-flex align-items-center mt-30" rel="noopener noreferrer">
            <div class="bolinha-whatsapp-conteudo ml-15 d-flex justify-content-center align-items-center bg-whatsapp">
              <i class="fab fa-whatsapp text-white fs-24" />
            </div>
            <div class="ml-2 mr-15 text-dark">
              <p class="fw-600 d-block fs-15 text-left mb-0 col-12 px-0">Norte de Santa Catarina</p>
              <p class="fw-600 d-block fs-15 text-left mb-0 col-12 px-0">(47) 99106-2096</p>
            </div>
            <div class="border-bottom col-12 mt-10" />
          </a>
          <a href="https://wa.me/5548998200602?text=Olá,+estou+visitando+o+site+da+Gaziella+Bastos+e+gostaria+de+receber+mais+informações" target="_blank" class="row mx-0 col-lg-6 col-xl-4 no-underline d-flex align-items-center mt-30" rel="noopener noreferrer">
            <div class="bolinha-whatsapp-conteudo ml-15 d-flex justify-content-center align-items-center bg-whatsapp">
              <i class="fab fa-whatsapp text-white fs-24" />
            </div>
            <div class="ml-2 mr-15 text-dark">
              <p class="fw-600 d-block fs-15 text-left mb-0 col-12 px-0">Sul de Santa Catarina</p>
              <p class="fw-600 d-block fs-15 text-left mb-0 col-12 px-0">(48) 99820-0602</p>
            </div>
            <div class="border-bottom col-12 mt-10" />
          </a>
          <a href="https://wa.me/5549991662520?text=Olá,+estou+visitando+o+site+da+Gaziella+Bastos+e+gostaria+de+receber+mais+informações" target="_blank" class="row mx-0 col-lg-6 col-xl-4 no-underline d-flex align-items-center mt-30" rel="noopener noreferrer">
            <div class="bolinha-whatsapp-conteudo ml-15 d-flex justify-content-center align-items-center bg-whatsapp">
              <i class="fab fa-whatsapp text-white fs-24" />
            </div>
            <div class="ml-2 mr-15 text-dark">
              <p class="fw-600 d-block fs-15 text-left mb-0 col-12 px-0">Serra Catarinense</p>
              <p class="fw-600 d-block fs-15 text-left mb-0 col-12 px-0">(49) 99166-2520</p>
            </div>
            <div class="border-bottom col-12 mt-10" />
          </a>
          <a href="https://wa.me/5541995190579?text=Olá,+estou+visitando+o+site+da+Gaziella+Bastos+e+gostaria+de+receber+mais+informações" target="_blank" class="row mx-0 col-lg-6 col-xl-4 no-underline d-flex align-items-center mt-30" rel="noopener noreferrer">
            <div class="bolinha-whatsapp-conteudo ml-15 d-flex justify-content-center align-items-center bg-whatsapp">
              <i class="fab fa-whatsapp text-white fs-24" />
            </div>
            <div class="ml-2 mr-15 text-dark">
              <p class="fw-600 d-block fs-15 text-left mb-0 col-12 px-0">Paraná</p>
              <p class="fw-600 d-block fs-15 text-left mb-0 col-12 px-0">(41) 99519-0579</p>
            </div>
            <div class="border-bottom col-12 mt-10" />
          </a>
          <a href="https://wa.me/5511973773244?text=Olá,+estou+visitando+o+site+da+Gaziella+Bastos+e+gostaria+de+receber+mais+informações" target="_blank" class="row mx-0 col-lg-6 col-xl-4 no-underline d-flex align-items-center mt-30" rel="noopener noreferrer">
            <div class="bolinha-whatsapp-conteudo ml-15 d-flex justify-content-center align-items-center bg-whatsapp">
              <i class="fab fa-whatsapp text-white fs-24" />
            </div>
            <div class="ml-2 mr-15 text-dark">
              <p class="fw-600 d-block fs-15 text-left mb-0 col-12 px-0">São Paulo</p>
              <p class="fw-600 d-block fs-15 text-left mb-0 col-12 px-0">(11) 97377-3244</p>
            </div>
            <div class="border-bottom col-12 mt-10" />
          </a>
          <a href="https://wa.me/5551997544960?text=Olá,+estou+visitando+o+site+da+Gaziella+Bastos+e+gostaria+de+receber+mais+informações" target="_blank" class="row mx-0 col-lg-6 col-xl-4 no-underline d-flex align-items-center mt-30" rel="noopener noreferrer">
            <div class="bolinha-whatsapp-conteudo ml-15 d-flex justify-content-center align-items-center bg-whatsapp">
              <i class="fab fa-whatsapp text-white fs-24" />
            </div>
            <div class="ml-2 mr-15 text-dark">
              <p class="fw-600 d-block fs-15 text-left mb-0 col-12 px-0">Rio Grande do Sul</p>
              <p class="fw-600 d-block fs-15 text-left mb-0 col-12 px-0">(51) 99754-4960</p>
            </div>
            <div class="border-bottom col-12 mt-10" />
          </a>
          <a href="https://wa.me/5521999932082?text=Olá,+estou+visitando+o+site+da+Gaziella+Bastos+e+gostaria+de+receber+mais+informações" target="_blank" class="row mx-0 col-lg-6 col-xl-4 no-underline d-flex align-items-center mt-30" rel="noopener noreferrer">
            <div class="bolinha-whatsapp-conteudo ml-15 d-flex justify-content-center align-items-center bg-whatsapp">
              <i class="fab fa-whatsapp text-white fs-24" />
            </div>
            <div class="ml-2 mr-15 text-dark">
              <p class="fw-600 d-block fs-15 text-left mb-0 col-12 px-0">Rio de Janeiro</p>
              <p class="fw-600 d-block fs-15 text-left mb-0 col-12 px-0">(21) 99993-2082</p>
            </div>
            <div class="border-bottom col-12 mt-10" />
          </a>
          <a href="https://wa.me/5531998082674?text=Olá,+estou+visitando+o+site+da+Gaziella+Bastos+e+gostaria+de+receber+mais+informações" target="_blank" class="row mx-0 col-lg-6 col-xl-4 no-underline d-flex align-items-center mt-30" rel="noopener noreferrer">
            <div class="bolinha-whatsapp-conteudo ml-15 d-flex justify-content-center align-items-center bg-whatsapp">
              <i class="fab fa-whatsapp text-white fs-24" />
            </div>
            <div class="ml-2 mr-15 text-dark">
              <p class="fw-600 d-block fs-15 text-left mb-0 col-12 px-0">Minas Gerais</p>
              <p class="fw-600 d-block fs-15 text-left mb-0 col-12 px-0">(31) 99808-2674</p>
            </div>
            <div class="border-bottom col-12 mt-10" />
          </a>
          <a href="https://wa.me/5562999599493?text=Olá,+estou+visitando+o+site+da+Gaziella+Bastos+e+gostaria+de+receber+mais+informações" target="_blank" class="row mx-0 col-lg-6 col-xl-4 no-underline d-flex align-items-center mt-30" rel="noopener noreferrer">
            <div class="bolinha-whatsapp-conteudo ml-15 d-flex justify-content-center align-items-center bg-whatsapp">
              <i class="fab fa-whatsapp text-white fs-24" />
            </div>
            <div class="ml-2 mr-15 text-dark">
              <p class="fw-600 d-block fs-15 text-left mb-0 col-12 px-0">Goiás</p>
              <p class="fw-600 d-block fs-15 text-left mb-0 col-12 px-0">(62) 99959-9493</p>
            </div>
            <div class="border-bottom col-12 mt-10" />
          </a>
          <a href="https://wa.me/5567996182861?text=Olá,+estou+visitando+o+site+da+Gaziella+Bastos+e+gostaria+de+receber+mais+informações" target="_blank" class="row mx-0 col-lg-6 col-xl-4 no-underline d-flex align-items-center mt-30" rel="noopener noreferrer">
            <div class="bolinha-whatsapp-conteudo ml-15 d-flex justify-content-center align-items-center bg-whatsapp">
              <i class="fab fa-whatsapp text-white fs-24" />
            </div>
            <div class="ml-2 mr-15 text-dark">
              <p class="fw-600 d-block fs-15 text-left mb-0 col-12 px-0">Mato Grosso do Sul</p>
              <p class="fw-600 d-block fs-15 text-left mb-0 col-12 px-0">(67) 99618-2861</p>
            </div>
            <div class="border-bottom col-12 mt-10" />
          </a>
          <a href="https://wa.me/5561998300643?text=Olá,+estou+visitando+o+site+da+Gaziella+Bastos+e+gostaria+de+receber+mais+informações" target="_blank" class="row mx-0 col-lg-6 col-xl-4 no-underline d-flex align-items-center mt-30" rel="noopener noreferrer">
            <div class="bolinha-whatsapp-conteudo ml-15 d-flex justify-content-center align-items-center bg-whatsapp">
              <i class="fab fa-whatsapp text-white fs-24" />
            </div>
            <div class="ml-2 mr-15 text-dark">
              <p class="fw-600 d-block fs-15 text-left mb-0 col-12 px-0">Distrito Federal</p>
              <p class="fw-600 d-block fs-15 text-left mb-0 col-12 px-0">(61) 99830-0643</p>
            </div>
            <div class="border-bottom col-12 mt-10" />
          </a>
        </div>
      </div>
    </b-modal>
  </div>
</template>
<script>
export default {
  created () {
    this.$root.$on('ShowModalWhatsapp', () => {
      this.$bvModal.show('modal-whatsapp')
    })
  }
}
</script>
<style scoped>
  .btn-fechar-modal{
    position: absolute;
    top: 0;
    right: 0;
  }
  .bolinha-whatsapp-conteudo{
    min-width: 40px;
    min-height: 40px;
    max-width: 40px;
    max-height: 40px;
    border-radius: 50%;
  }
  .bg-whatsapp{
    background-color: #34af23;
  }
  .bg-whatsapp:hover{
    background-color: #288f1a;
  }
</style>
