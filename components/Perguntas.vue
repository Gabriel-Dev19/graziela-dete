<template>
  <div class="bg-roxo-escuro position-relative d-flex justify-content-center overflow-hidden pb-40 mt-140">
    <div class="borda-cima" />
    <div class="container">
      <h1 class="font-teko position-relative col-xs-8 mx-auto col-sm-12 d-flex justify-content-center text-uppercase text-center">
        Perguntas frequentes
        <div class="separation-tema" />
      </h1>
      <div class="d-flex row justify-content-center align-items-start mx-auto mt-120">
        <div class="py-2 mt-20 bg-light w-perguntas">
          <button v-b-toggle.perguntas-1 class="btn fw-600 px-15 d-flex text-left justify-content-between align-items-center col-12">
            Quais os diferenciais nos serviços prestados e nas investigações conduzidas pelos
            detetives particulares da Agência de Detetives Graziella Bastos em relação
            aos concorrentes? <ion-icon class="text-roxo-escuro pr-0 fs-23 ml-4" name="add-circle-outline" />
          </button>
          <b-collapse id="perguntas-1">
            <p class="px-3 pt-10 mb-2">
              Transparência em todo o processo, qualidade do material apresentado,
              procedimentos de segurança para preservar o sigilo dos nossos clientes.
            </p>
          </b-collapse>
        </div>
        <div class="py-2 mt-20 bg-light w-perguntas">
          <button v-b-toggle.perguntas-2 class="btn fw-600 px-15 d-flex text-left justify-content-between align-items-center col-12">
            Quais as formas de pagamento? <ion-icon class="text-roxo-escuro pr-0 fs-23 ml-4" name="add-circle-outline" />
          </button>
          <b-collapse id="perguntas-2">
            <p class="px-3 pt-10 mb-2">
              Por padrão, 50% ato e o restante na entrega dos resultados da investigação realizada pelo detetive particular. Em alguns casos, os clientes dividem em até 03 vezes no cartão de crédito.
            </p>
          </b-collapse>
        </div>
        <div class="py-2 mt-20 bg-light w-perguntas">
          <button v-b-toggle.perguntas-3 class="btn fw-600 px-15 d-flex text-left justify-content-between align-items-center col-12">
            Já aconteceu de alguma pessoa investigada descobrir a investigação? Se sim, como proceder nesse caso? <ion-icon class="text-roxo-escuro pr-0 fs-23 ml-4" name="add-circle-outline" />
          </button>
          <b-collapse id="perguntas-3">
            <p class="px-3 pt-10 mb-2">
              Certamente esse é um risco que estamos expostos no decorrer da investigação, porém nossos detetives são devidamente treinados e capacitados para poderem se sobressair a qualquer situação. Todos esses procedimentos são informados ao cliente no ato da contratação e, em caso de risco, o trabalho é abortado no momento para garantir a continuidade do mesmo posteriormente.
            </p>
            <p class="px-3 pt-10 mb-2">
              Em situações de investigação conjugal ou familiar, o próprio cliente pode acabar deixando escapar que está investigando devido à ansiedade que vai sendo gerada no decorrer dos trabalhos. É necessário manter o comportamento normal até o final das investigações.
            </p>
            <p class="px-3 pt-10 mb-2">
              É recomendado mudar todas as senhas dos dispositivos e contas de e-mails. Ou até mesmo criar um e-mail novo somente para receber o material do resultado das investigações.
            </p>
          </b-collapse>
        </div>
        <div class="py-2 mt-20 bg-light w-perguntas">
          <button v-b-toggle.perguntas-4 class="btn fw-600 px-15 d-flex text-left justify-content-between align-items-center col-12">
            Quais as fases da investigação conjugal? <ion-icon class="text-roxo-escuro pr-0 fs-23 ml-4" name="add-circle-outline" />
          </button>
          <b-collapse id="perguntas-4">
            <p class="px-3 pt-10 mb-2">
              A investigação conjugal não tem um padrão, varia de acordo com cada alvo. Em alguns casos, o cliente já chega até o detetive particular com muita informação e o que precisa é somente da prova que é uma foto ou filmagem.
            </p>
            <p class="px-3 pt-10 mb-2">
              Em outras situações, alguns começam utilizando equipamentos para monitoramento, fazendo uma análise prévia do comportamento, ouvindo conversas e verificando atividades.
            </p>
            <p class="px-3 pt-10 mb-2">
              Em alguns casos o cliente inicia procurando uma infidelidade e descobre algo mais grave como planos de golpes financeiros, e até mesmo planos contra a vida do cliente.
            </p>
          </b-collapse>
        </div>
        <div class="py-2 mt-20 bg-light w-perguntas">
          <button v-b-toggle.perguntas-5 class="btn fw-600 px-15 d-flex text-left justify-content-between align-items-center col-12">
            O que a pessoa que contrata o serviço precisa fazer para ajudar o detetive particular em uma investigação conjugal? <ion-icon class="text-roxo-escuro pr-0 fs-23 ml-4" name="add-circle-outline" />
          </button>
          <b-collapse id="perguntas-5">
            <p class="px-3 pt-10 mb-2">
              É importante deixar bem claro qual é o objetivo principal e, é claro, passar as informações básicas de forma correta para o detetive particular.
            </p>
          </b-collapse>
        </div>
        <div class="py-2 mt-20 bg-light w-perguntas">
          <button v-b-toggle.perguntas-6 class="btn fw-600 px-15 d-flex text-left justify-content-between align-items-center col-12">
            Em média, quanto tempo leva uma investigação conjugal, empresarial e familiar? <ion-icon class="text-roxo-escuro pr-0 fs-23 ml-4" name="add-circle-outline" />
          </button>
          <b-collapse id="perguntas-6">
            <p class="px-3 pt-10 mb-2">
              As investigações conjugais e familiares costumam levar, em média, de 05 a 10 dias. Já a investigação
              empresarial dura de 05 a 60 dias. Mas, obviamente, esse tempo pode variar de acordo com cada caso e
              com o processo investigativo realizado pelo detetive particular.
            </p>
          </b-collapse>
        </div>
        <div class="py-2 mt-20 bg-light w-perguntas">
          <button v-b-toggle.perguntas-7 class="btn fw-600 px-15 d-flex text-left justify-content-between align-items-center col-12">
            Quando uma criança/adolescente desaparece, qual a primeira coisa que o detetive particular faz? <ion-icon class="text-roxo-escuro pr-0 fs-23 ml-4" name="add-circle-outline" />
          </button>
          <b-collapse id="perguntas-7">
            <p class="px-3 pt-10 mb-2">
              A primeira recomendação é procurar a polícia e fazer o boletim de ocorrência. O serviço do detetive particular é algo adicional.
            </p>
            <p class="px-3 pt-10 mb-2">
              A primeira é colher todas as informações que os pais se lembram da última vez que viram a pessoa desaparecida, como horário, comportamento e trajes. Depois, o detetive particular conversa com pessoas do local, realiza uma varredura no ambiente e busca por imagens de câmeras de segurança.
            </p>
          </b-collapse>
        </div>
        <div class="py-2 mt-20 bg-light w-perguntas">
          <button v-b-toggle.perguntas-8 class="btn fw-600 px-15 d-flex text-left justify-content-between align-items-center col-12">
            Quando os pais estão investigando filhos adolescentes, quais são as descobertas mais comuns? <ion-icon class="text-roxo-escuro pr-0 fs-23 ml-4" name="add-circle-outline" />
          </button>
          <b-collapse id="perguntas-8">
            <p class="px-3 pt-10 mb-2">
              O mais comum entre adolescentes, que é descoberto pelos detetives particulares, é o uso de entorpecentes e a prática de atividades ilícitas.
            </p>
          </b-collapse>
        </div>
        <div class="py-2 mt-20 bg-light w-perguntas">
          <button v-b-toggle.perguntas-9 class="btn fw-600 px-15 d-flex text-left justify-content-between align-items-center col-12">
            Geralmente quais são as principais pistas encontradas em um caso de investigação de funcionários/empresarial? <ion-icon class="text-roxo-escuro pr-0 fs-23 ml-4" name="add-circle-outline" />
          </button>
          <b-collapse id="perguntas-9">
            <p class="px-3 pt-10 mb-2">
              Normalmente o cliente/vítima procura um detetive particular, pois está tendo desvios de alguma forma. As pistas variam de acordo com o cargo do funcionário.
            </p>
            <p class="px-3 pt-10 mb-2">
              Investigando a rotina desses funcionários, o que chama atenção é o estilo de vida incompatível com a remuneração. Além de atividades dos funcionários em endereços de concorrentes e reuniões com pessoas estranhas. Tudo é investigado em detalhes.
            </p>
          </b-collapse>
        </div>
        <div class="py-2 mt-20 bg-light w-perguntas">
          <button v-b-toggle.perguntas-10 class="btn fw-600 px-15 d-flex text-left justify-content-between align-items-center col-12">
            Quais os principais sinais que motivam uma empresa contratar a contrainteligência? <ion-icon class="text-roxo-escuro pr-0 fs-23 ml-4" name="add-circle-outline" />
          </button>
          <b-collapse id="perguntas-10">
            <p class="px-3 pt-10 mb-2">
              Empresas que participam de licitação e que não conseguem sucesso costumam procurar serviços de varreduras em busca de escutas.
            </p>
            <p class="px-3 pt-10 mb-2">
              Casos de sabotagem no departamento de produção.
            </p>
            <p class="px-3 pt-10 mb-2">
              Concorrências desleais e furto de dados sensíveis por ex-funcionários entre outros casos.
            </p>
          </b-collapse>
        </div>
        <div class="py-2 mt-20 bg-light w-perguntas">
          <button v-b-toggle.perguntas-11 class="btn fw-600 px-15 d-flex text-left justify-content-between align-items-center col-12">
            Afinal, o Celular VIP consegue quais informações do investigado? <ion-icon class="text-roxo-escuro pr-0 fs-23 ml-4" name="add-circle-outline" />
          </button>
          <b-collapse id="perguntas-11">
            <p class="px-3 pt-10 mb-2">
              O Celular VIP é um programa que será instalado no celular do alvo realizando cópias das comunicações de vários aplicativos de conversas e localização. Você consegue controlar o celular a distância, basta estar ligado e conectado na internet.
            </p>
          </b-collapse>
        </div>
        <div class="d-flex col-12 mt-50 justify-content-center">
          <button class="btn btn-perguntas text-uppercase fs-14 py-10 px-25 border-radius-30 fw-600" @click.prevent="ScrollContato">
            Faça uma pergunta
          </button>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data () {
    return {
      Quantidade_retira_hash: 0
    }
  },
  methods: {
    ScrollContato () {
      this.$smoothScroll({
        scrollTo: document.getElementById('contato'),
        duration: 500,
        offset: -10
      })
      setTimeout(() => {
        this.HideHash()
      }, 490)
    },
    HideHash () {
      this.Quantidade_retira_hash = 0
      const interval = setInterval(() => {
        let scrollV; let scrollH; const loc = window.location
        if ('replaceState' in history) {
          history.replaceState('', document.title, loc.pathname + loc.search)
        } else {
          // Prevent scrolling by storing the page's current scroll offset
          scrollV = document.body.scrollTop
          scrollH = document.body.scrollLeft
          loc.hash = ''
          // Restore the scroll offset, should be flicker free
          document.body.scrollTop = scrollV
          document.body.scrollLeft = scrollH
        }
        this.Quantidade_retira_hash++
        if (this.Quantidade_retira_hash > 15) { clearInterval(interval) }
      }, 0)
    }
  }
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
  ion-icon.fs-23{
    min-width: 23px;
    min-height: 23px;
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
    .w-perguntas{
      width: 80%;
    }
  }
  .separation-tema{
    position: absolute;
    height: 3px;
    width: 150px;
    bottom: -10px;
    border-radius: 3px;
    background-color: var(--roxo_escuro);
  }
</style>
