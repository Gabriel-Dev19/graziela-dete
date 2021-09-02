<template>
  <div>
    <Home title-home="Celular VIP - Monitore tudo!" name-btn-home-servicos="Outros serviços" :bg-software="true" />
    <section class="pt-100">
      <div class="container">
        <h1 class="font-teko position-relative col-12 px-0 d-flex justify-content-center text-uppercase text-center">
          Mais sobre o Celular VIP
          <div class="separation-tema" />
        </h1>
        <div class="mt-50 row mx-auto d-xs-flex d-sm-block">
          <div class="col-sm-5 col-md-4 col-lg-3 px-0 mt-xs-50 ml-sm-30 mb-sm-30 order-2 float-sm-right">
            <h5 class="fw-600 text-xs-center text-roxo-escuro">
              Investigação com riqueza de detalhes!
            </h5>
            <p class="fs-14 text-xs-center fw-500">
              Detalhamos a investigação completa e fornecemos
              tudo documentado.
            </p>
            <div class="position-relative">
              <div class="borda-lateral-sobre d-xs-none" />
              <div class="d-flex row mx-auto justify-content-xs-center">
                <ion-icon class="fs-24 bg-light order-xs-2 mt-xs-1 text-roxo-escuro" name="chevron-down-circle-outline" style="margin-top: -2px; --ionicon-stroke-width: 23px;" />
                <span class="fs-14 col-xs-12 text-xs-center order-xs-1 fw-500 ml-1">Diagnóstico</span>
              </div>
              <div class="d-flex row mx-auto justify-content-xs-center mt-15">
                <ion-icon class="fs-24 bg-light order-xs-2 mt-xs-1 text-roxo-escuro" name="chevron-down-circle-outline" style="margin-top: -2px; --ionicon-stroke-width: 23px;" />
                <span class="fs-14 col-xs-12 text-xs-center order-xs-1 fw-500 ml-1">Instalação do software</span>
              </div>
              <div class="d-flex row mx-auto justify-content-xs-center mt-15">
                <ion-icon class="fs-24 bg-light order-xs-2 mt-xs-1 text-roxo-escuro" name="chevron-down-circle-outline" style="margin-top: -2px; --ionicon-stroke-width: 23px;" />
                <span class="fs-14 col-xs-12 text-xs-center order-xs-1 fw-500 ml-1">Monitoramento do celular</span>
              </div>
              <div class="d-flex row mx-auto justify-content-xs-center mt-15">
                <ion-icon class="fs-24 bg-light order-xs-2 mt-xs-1 text-roxo-escuro" name="chevron-down-circle-outline" style="margin-top: -2px; --ionicon-stroke-width: 23px;" />
                <span class="fs-14 col-xs-12 text-xs-center order-xs-1 fw-500 ml-1">Preparação do dossiê</span>
              </div>
              <div class="d-flex row mx-auto justify-content-xs-center mt-15">
                <ion-icon class="fs-24 bg-light order-xs-2 mt-xs-1 text-roxo-escuro" name="checkmark-circle" style="margin-top: -2px; --ionicon-stroke-width: 23px;" />
                <span class="fs-14 col-xs-12 text-xs-center order-xs-1 fw-500 ml-1">A verdade na suas mãos!</span>
              </div>
            </div>
            <div class="d-flex justify-content-xs-center">
              <BtnRoxoContatoScroll class="mt-4" name-btn="Faça uma consulta" />
            </div>
          </div>
          <p class="fw-500 col-xs-12 px-0 text-xs-center text-sm-left">
            Obtenha acesso remoto a todas as atividades do celular do seu filho. Todas as informações são armazenadas de modo seguro e protegido, apenas você terá acesso a elas.
          </p>
          <p class="fw-500 col-xs-12 px-0 text-xs-center text-sm-left">
            Trabalhamos com o Celular VIP desde 2011, ajudando milhares de pessoas e empresas que utilizam deste serviço. Prezamos pela segurança de sua família e/ou empresa, somos pioneiros a disponibilizar esses serviços no mercado.
          </p>
          <p class="fw-500 col-xs-12 px-0 text-xs-center text-sm-left">
            Esclareça suas dúvidas com a nossa equipe de suporte. Com o Celular VIP, você não ficará sozinho com suas dúvidas ou dificuldades.
          </p>
          <p class="fw-500 col-xs-12 px-0 text-xs-center text-sm-left">
            Com o nosso Celular VIP para o monitoramento de filhos você terá acesso a uma ferramenta de proteção dos filhos bastante eficiente, considerando-se os riscos aos quais crianças e adolescentes estão expostos, tanto no mundo real como no virtual.
          </p>
          <p class="fw-500 col-xs-12 px-0 text-xs-center text-sm-left">
            Seus filhos estão constantemente expostos ao risco de andar com más companhias que os induzam à prática de atividades ilícitas, a sequestros, raptos, exploração infantil, incentivadores de suicídios virtuais, dentre outras atrocidades. É dever dos pais proteger os filhos contra tais riscos.
          </p>
          <p class="fw-500 col-xs-12 px-0 text-xs-center text-sm-left">
            Foi pensando na mitigação destes riscos familiares que a Agência de Detetives Graziella Bastos idealizou em seu portfólio de serviços de Detetive Particular o Celular VIP. Trata-se de uma ferramenta eficaz no monitoramento de filhos e sua utilização de dispositivos eletrônicos tais como celulares, tablets e computadores.
            Consulte-nos acerca das funcionalidades do Celular VIP. Adquira sua tranquilidade!
          </p>
          <h1 class="font-teko text-xs-center text-sm-center text-lg-left mt-40 d-flex justify-content-xs-center justify-content-sm-center justify-content-lg-start position-relative mb-1">
            Funções do celular VIP
            <div class="borda-tema-fina" />
          </h1>
          <div class="row mx-auto">
            <div v-for="funcao in funcoes" :key="funcao.title_funcao" class="w-funcoes-celular-vip d-flex">
              <ion-icon class="text-roxo" :name="funcao.icon" />
              <div class="col px-0 ml-3">
                <h6 class="fw-600">
                  {{ funcao.title_funcao }}
                </h6>
                <p class="fs-15">
                  {{ funcao.text_funcao }}
                </p>
              </div>
            </div>
          </div>
          <h1 class="font-teko text-xs-center text-sm-center text-lg-left mt-50 d-flex justify-content-xs-center justify-content-sm-center justify-content-lg-start position-relative mb-1">
            A iportância do monitoramento
            <div class="borda-tema-fina" />
          </h1>
          <p class="fw-500 col-xs-12 mt-20 px-0 text-xs-center text-sm-left">
            Como os pais sabem se os filhos estão envolvidos em atividades virtuais inapropriadas para eles? E como você saberia se a sua criança ou o seu adolescente foi vítima de abuso se ela(e) não lhe disser? E se essas atividades ultrapassarem os limites virtuais e seu(sua) filho(a) for ao encontro de algum delinquente? Veja, a seguir, outros perigos aos quais seus filhos estão expostos e que podem ser mitigados por um Detetive Particular.
          </p>
          <div class="d-flex justify-content-center justify-content-lg-start">
            <BtnRoxoContatoScroll class="mt-2" name-btn="Monitore agora!" />
          </div>
        </div>
      </div>
    </section>
    <Servicos title-servicos="Outros serviços" class="mt-150" :hide-software="false" />
  </div>
</template>

<script>
import BtnRoxoContatoScroll from '~/components/buttons/BtnRoxoContatoScroll.vue'
import Home from '~/components/Home.vue'
import Servicos from '~/components/Servicos.vue'
export default {
  components: { Home, Servicos, BtnRoxoContatoScroll },
  layout: 'LayoutServicos',
  data () {
    return {
      funcoes: [
        {
          title_funcao: 'Mensageiros',
          text_funcao: `Tenha acesso a todas as informações (mensagens de textos e áudios) das
          redes sociais do Whatsapp, Snapchat, iMessage, Skype, Telegram, Viber, Hangout, LINE, etc.`,
          icon: 'logo-whatsapp'
        },
        {
          title_funcao: 'Ligações',
          text_funcao: `Todas as chamadas recebidas e realizadas com horários,
          duração e informações sobre a pessoa`,
          icon: 'call-outline'
        },
        {
          title_funcao: 'SMS',
          text_funcao: `Todas as mensagens de texto enviadas, recebidas ou deletadas
          com horários e informações sobre o contato`,
          icon: 'chatbubbles-outline'
        },
        {
          title_funcao: 'Localização em tempo real',
          text_funcao: `Localização atual no mapa, rotas e
          locais visitados`,
          icon: 'location-outline'
        },
        {
          title_funcao: 'Histórico de navegação',
          text_funcao: `Todo o histórico e atividades do navegador
          da web com horários e favoritos`,
          icon: 'list-outline'
        },
        {
          title_funcao: 'Apps sociais',
          text_funcao: `Facebook, Instagram,
          Tinder, etc.`,
          icon: 'logo-facebook'
        },
        {
          title_funcao: 'Fotos e vídeos',
          text_funcao: `Todos os arquivos de mídia compartilhados,
          recebidos, baixados ou armazenados no dispositivo.`,
          icon: 'images-outline'
        },
        {
          title_funcao: 'Outras atividades',
          text_funcao: `Contatos, Calendário, E-mail, Apps
          Instalados, redes de Wi-Fi e mais.`,
          icon: 'settings-outline'
        }
      ]
    }
  },
  head: {
    title: 'Celular VIP - Monitore tudo! - Agência de detetives Graziella Bastos'
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
    bottom: -5px;
    border-radius: 3px;
    background-color: var(--roxo_escuro);
  }
  @media (max-width: 768px) {
    .w-funcoes-celular-vip{
      width: 100%;
      margin-top: 50px;
    }
  }
  @media (min-width: 768px) and (max-width: 1200px) {
    .w-funcoes-celular-vip{
      width: 45%;
      margin-top: 50px;
    }
    .w-funcoes-celular-vip:nth-child(2n+1){
      margin-right: 10%;
    }
  }
  @media (min-width: 1200px) {
    .w-funcoes-celular-vip{
      width: 31%;
      margin-top: 50px;
    }
    .w-funcoes-celular-vip:nth-child(3n+2){
      margin-right: 3.5%;
      margin-left: 3.5%;
    }
  }
  .w-funcoes-celular-vip ion-icon{
    font-size: 45px;
    min-width: 45px;
  }
  .borda-lateral-sobre{
    position: absolute;
    height: 100%;
    top: 0;
    left: 12px;
    z-index: -3;
    border-left: 1px solid var(--roxo_escuro);
  }
</style>
