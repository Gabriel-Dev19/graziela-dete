<template>
  <div>
    <Home title-home="Sobre a agência Graziella Bastos" :bg-home="true" />
    <section class="pt-100">
      <div class="container">
        <h1 class="font-teko position-relative col-12 px-0 d-flex justify-content-center text-uppercase text-center">
          Saiba mais sobre Graziella e sua equipe
          <div class="separation-tema" />
        </h1>
        <div class="d-flex justify-content-between align-items-start row mx-auto mt-80">
          <div class="col-lg-6 col-xl-7 px-0">
            <h1 class="font-teko d-flex justify-content-xs-center justify-content-sm-center justify-content-lg-start position-relative mb-1">
              Quem somos?
              <div class="borda-tema-fina" />
            </h1>
            <p class="mt-30 text-xs-center text-sm-center text-lg-left fw-500 px-0">
              A Agência de Detetives Graziella Bastos está no mercado da Investigação Particular desde 2006, são 15 anos de atuação dedicando-se em investigações na área particular e empresarial.
            </p>
            <p class="text-xs-center text-sm-center text-lg-left fw-500 px-0">
              Atendemos em todo território nacional com escritórios nas principais cidades de cada região. Dedicamos a nossa experiência aos particulares e às empresas que procuram um serviço de investigação privada com base na integridade, competência, e profissionalismo, empenhando os nossos esforços com objetividade e eficiência. As investigações propostas são convenientemente analisadas caso a caso, atendendo às suas circunstâncias e grau de dificuldade. O sigilo e a confidencialidade são assegurados como elementos primordiais nos serviços prestados ao cliente.
            </p>
            <h1 class="font-teko text-xs-center text-sm-center text-lg-left mt-40 d-flex justify-content-xs-center justify-content-sm-center justify-content-lg-start position-relative mb-1">
              Transparência e qualidade na investigação
              <div class="borda-tema-fina" />
            </h1>
            <p class="mt-30 text-xs-center text-sm-center text-lg-left fw-500 px-0">
              Nós, independentemente do tipo de investigação, nos destacamos pela transparência em nossos serviços. Buscamos deixar o cliente por dentro de tudo que está acontecendo, tendo à disposição uma total abertura a respeito de cada procedimento realizado.
            </p>
            <p class="text-xs-center text-sm-center text-lg-left fw-500 px-0">
              Ao finalizarmos o caso, oferecemos ao cliente, provas, das mais variadas mídias, como fotos, áudios e vídeos, tudo de altíssima qualidade. Tudo devidamente escrito sob a forma da lei para serem utilizadas em processos judiciais futuros. Somos inscritos junto aos órgãos competentes, logo garantimos a plena confidencialidade de cada caso, sejam os encerrados ou os em andamento.
            </p>
            <h1 class="font-teko mt-40 text-xs-center text-sm-center text-lg-left d-flex justify-content-xs-center justify-content-sm-center justify-content-lg-start position-relative mb-1">
              Serviços de detetive particular 24 horas
              <div class="borda-tema-fina" />
            </h1>
            <p class="mt-30 text-xs-center text-sm-center text-lg-left fw-500 px-0">
              Com uma equipe de detetives especializados e qualificados que seguem o código de ética da profissão, o trabalho da Agência de Detetives Graziella Bastos é apresentar uma solução para o problema de seus clientes, por meio de provas reais (imagens, áudios e documentos) que comprovem ou não a suspeita, com total certeza e máximo sigilo.
            </p>
            <h1 class="font-teko mt-40 text-xs-center text-sm-center text-lg-left d-flex justify-content-xs-center justify-content-sm-center justify-content-lg-start position-relative mb-1">
              Investigação particular
              <div class="borda-tema-fina" />
            </h1>
            <p class="mt-30 text-xs-center text-sm-center text-lg-left fw-500 px-0">
              A investigação particular tem no seu campo de atuação os mais variados interesses. O sigilo é regra de ouro para a Agência de Detetives Graziella Bastos, os assuntos dos nossos clientes que respeitam ao foro pessoal são tidos em conta com o máximo sigilo e confidencialidade, tratando-se de segredos invioláveis e absolutamente intransmissíveis. Caso não encontre o seu caso especifico abaixo descrito não hesite em contatar-nos.
            </p>
            <p class="text-xs-center text-sm-center text-lg-left fw-500 px-0">
              Nosso serviço investigação particular, conta com o trabalho de detetives altamente capacitados e treinados, prontos para orientar nosso cliente e ajudar solucionar os seus problemas.  Toda a estratégia de investigação será devidamente planejada junto com nosso cliente, a fim de termos êxito em nossa investigação. Lembrando que cada caso é um caso.
            </p>
            <p class="text-xs-center text-sm-center text-lg-left fw-500 px-0">
              Atuando com total sigilo e cautela, os nossos detetives, afim de proporcionar segurança ao cliente, durante toda a investigação particular, ele será informado sobre o que está acontecendo e o que está sendo feito.
            </p>
            <p class="text-xs-center text-sm-center text-lg-left fw-500 px-0">
              Garantimos total segurança e privacidade ao cliente, e em nenhum momento iremos expor o contratante em situações que podem deixá-lo em perigo.
            </p>
            <div class="d-flex justify-content-xs-center justify-content-sm-center mt-4 justify-content-lg-start">
              <btn-roxo-contato-scroll name-btn="Entre em contato" />
            </div>
          </div>
          <div class="col-lg ml-lg-90 mt-xs-70 mt-sm-70 mt-lg-0 px-0">
            <card-sobre />
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import BtnRoxoContatoScroll from '~/components/buttons/BtnRoxoContatoScroll.vue'
import Home from '~/components/Home.vue'
import CardSobre from '~/components/parts/CardSobre.vue'
export default {
  components: { Home, BtnRoxoContatoScroll, CardSobre },
  layout: 'LayoutSobre',
  head: {
    title: 'Sobre nós - Agência de detetives Graziella Bastos'
  },
  mounted () {
    this.$smoothScroll({
      scrollTo: document.body,
      duration: 0,
      offset: 0
    })
    this.HideHash()
  },
  methods: {
    HideHash () {
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
    }
  }
}
</script>
<style scoped>
  .separation-tema{
    position: absolute;
    height: 3px;
    width: 200px;
    bottom: -10px;
    border-radius: 3px;
    background-color: var(--roxo_escuro);
  }
  .borda-tema-fina{
    position: absolute;
    height: 2px;
    width: 200px;
    bottom: -1px;
    border-radius: 3px;
    background-color: var(--roxo_escuro);
  }
  ol.carousel-indicators li{
    width: 13px !important;
    height: 13px !important;
  }
</style>
