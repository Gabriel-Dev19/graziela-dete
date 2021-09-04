<template>
  <div>
    <header>
      <nav v-scroll="ScrollNav" class="navbar align-items-center px-0 d-lg-none fixed-top nav" :class="{'bg-nav-scroll py-0 shadow': NavScroll, 'pt-40': !NavScroll}">
        <div class="container px-30" :class="{'border-bottom pt-15 pb-15': CollapseNav, 'pt-10 pb-10': NavScroll}">
          <a href="https://detetivegraziella.com.br" :class="{'text-white': !NavScroll, 'text-grafite': NavScroll}">
            <img v-show="!NavScroll" src="../assets/img/logo-grazi.webp" width="70" alt="Logo Graziela Detetives">
            <img v-show="NavScroll" src="../assets/img/logo-chapeu.webp" width="40" alt="Logo Graziela Detetives">
          </a>
          <button v-b-toggle.collapse-navbar class="btn py-0 px-0">
            <ion-icon v-show="IconBar" class="fs-40 text-roxo" name="menu-outline" style="margin-bottom: -7px;" />
            <ion-icon v-show="IconTimes" class="fs-37 text-roxo" name="close-circle-outline" style="margin-bottom: -7px;" />
          </button>
        </div>
        <b-collapse id="collapse-navbar" class="col-12 px-0">
          <div class="nav-event col-12 pb-40 bg-light">
            <h3 class="font-teko mt-3">
              Menu principal
            </h3>
            <div class="pl-10">
              <button v-b-toggle.collapse-navbar class="btn py-0 fw-500 fs-18 px-0 text-left d-flex align-items-center" @click.prevent="$router.push('/')">
                Página inicial <i class="fa fa-arrow-right text-roxo fs-15 ml-2" style="margin-top: 2px;" />
              </button>
              <button v-b-toggle.collapse-navbar class="btn py-0 fw-500 mt-2 fs-18 px-0 text-left d-flex align-items-center" @click.prevent="$router.push('/sobre/')">
                Sobre nós <i class="fa fa-arrow-right text-roxo fs-15 ml-2" style="margin-top: 2px;" />
              </button>
              <button v-b-toggle.collapse-servicos class="btn py-0 fw-500 mt-2 fs-18 px-0 text-left d-flex align-items-center">
                Serviços <i class="fa fa-angle-down text-roxo fs-15 ml-2" style="margin-top: 2px;" />
              </button>
              <b-collapse id="collapse-servicos">
                <div class="pl-30 pb-10 pt-1">
                  <button v-b-toggle.collapse-navbar class="btn py-0 fw-500 fs-18 px-0 text-left d-flex align-items-center" @click.prevent="$router.push('/servicos/')">
                    Todos os serviços <i class="fa fa-arrow-right text-roxo fs-15 ml-2" style="margin-top: 2px;" />
                  </button>
                  <button v-b-toggle.collapse-navbar class="btn py-0 fw-500 fs-18 px-0 text-left d-flex align-items-center" @click.prevent="$router.push('/servicos/investigacao-conjugal/')">
                    Investigação conjugal <i class="fa fa-arrow-right text-roxo fs-15 ml-2" style="margin-top: 2px;" />
                  </button>
                  <button v-b-toggle.collapse-navbar class="btn py-0 fw-500 fs-18 px-0 text-left d-flex align-items-center" @click.prevent="$router.push('/servicos/investigacao-empresarial/')">
                    Investigação empresarial <i class="fa fa-arrow-right text-roxo fs-15 ml-2" style="margin-top: 2px;" />
                  </button>
                  <button v-b-toggle.collapse-navbar class="btn py-0 fw-500 fs-18 px-0 text-left d-flex align-items-center" @click.prevent="$router.push('/servicos/comportamento-de-filhos/')">
                    Comportamento de filhos <i class="fa fa-arrow-right text-roxo fs-15 ml-2" style="margin-top: 2px;" />
                  </button>
                  <button v-b-toggle.collapse-navbar class="btn py-0 fw-500 fs-18 px-0 text-left d-flex align-items-center" @click.prevent="$router.push('/servicos/localizacao-de-pessoas/')">
                    Localização de pessoas <i class="fa fa-arrow-right text-roxo fs-15 ml-2" style="margin-top: 2px;" />
                  </button>
                  <button v-b-toggle.collapse-navbar class="btn py-0 fw-500 fs-18 px-0 text-left d-flex align-items-center" @click.prevent="$router.push('/servicos/provas-para-advogados/')">
                    Provas para advogados <i class="fa fa-arrow-right text-roxo fs-15 ml-2" style="margin-top: 2px;" />
                  </button>
                  <button v-b-toggle.collapse-navbar class="btn py-0 fw-500 fs-18 px-0 text-left d-flex align-items-center" @click.prevent="$router.push('/servicos/celular-VIP/')">
                    Celular VIP <i class="fa fa-arrow-right text-roxo fs-15 ml-2" style="margin-top: 2px;" />
                  </button>
                </div>
              </b-collapse>
              <button v-b-toggle.collapse-localidades class="btn py-0 fw-500 mt-2 fs-18 px-0 text-left d-flex align-items-center">
                Onde atendemos <i class="fa fa-angle-down text-roxo fs-15 ml-2" style="margin-top: 2px;" />
              </button>
              <b-collapse id="collapse-localidades">
                <div class="pl-30 pb-10 pt-1">
                  <button v-b-toggle.collapse-navbar class="btn py-0 fw-500 fs-18 px-0 text-left d-flex align-items-center" @click.prevent="$router.push('/detetive-particular-em-Santa-Catarina')">
                    <i class="fa fa-map-marker-alt mr-2 fs-13 text-roxo" /> Santa Catarina
                  </button>
                  <button v-b-toggle.collapse-navbar class="btn py-0 fw-500 fs-18 px-0 text-left d-flex align-items-center" @click.prevent="$router.push('/detetive-particular-no-Parana')">
                    <i class="fa fa-map-marker-alt mr-2 fs-13 text-roxo" /> Paraná
                  </button>
                  <button v-b-toggle.collapse-navbar class="btn py-0 fw-500 fs-18 px-0 text-left d-flex align-items-center" @click.prevent="$router.push('/detetive-particular-no-Rio-Grande-do-Sul')">
                    <i class="fa fa-map-marker-alt mr-2 fs-13 text-roxo" /> Rio Grande do Sul
                  </button>
                  <button v-b-toggle.collapse-navbar class="btn py-0 fw-500 fs-18 px-0 text-left d-flex align-items-center" @click.prevent="$router.push('/detetive-particular-em-Sao-Paulo')">
                    <i class="fa fa-map-marker-alt mr-2 fs-13 text-roxo" /> São Paulo
                  </button>
                  <button v-b-toggle.collapse-navbar class="btn py-0 fw-500 fs-18 px-0 text-left d-flex align-items-center" @click.prevent="$router.push('/detetive-particular-no-Rio-de-Janeiro')">
                    <i class="fa fa-map-marker-alt mr-2 fs-13 text-roxo" /> Rio de Janeiro
                  </button>
                  <button v-b-toggle.collapse-navbar class="btn py-0 fw-500 fs-18 px-0 text-left d-flex align-items-center" @click.prevent="$router.push('/detetive-particular-no-Distrito-Federal')">
                    <i class="fa fa-map-marker-alt mr-2 fs-13 text-roxo" /> Distrito Federal
                  </button>
                  <button v-b-toggle.collapse-navbar class="btn py-0 fw-500 fs-18 px-0 text-left d-flex align-items-center" @click.prevent="$router.push('/detetive-particular-em-Minas-Gerais')">
                    <i class="fa fa-map-marker-alt mr-2 fs-13 text-roxo" /> Minas Gerais
                  </button>
                  <button v-b-toggle.collapse-navbar class="btn py-0 fw-500 fs-18 px-0 text-left d-flex align-items-center" @click.prevent="$router.push('/detetive-particular-no-Mato-Grosso-do-Sul')">
                    <i class="fa fa-map-marker-alt mr-2 fs-13 text-roxo" /> Mato Grosso do Sul
                  </button>
                  <button v-b-toggle.collapse-navbar class="btn py-0 fw-500 fs-18 px-0 text-left d-flex align-items-center" @click.prevent="$router.push('/detetive-particular-em-Goias')">
                    <i class="fa fa-map-marker-alt mr-2 fs-13 text-roxo" /> Goiás
                  </button>
                </div>
              </b-collapse>
              <button v-b-toggle.collapse-navbar class="btn py-0 fw-500 mt-2 fs-18 px-0 text-left d-flex align-items-center" @click.prevent="ScrollContato">
                Fale conosco <i class="fa fa-arrow-right text-roxo fs-15 ml-2" style="margin-top: 2px;" />
              </button>
            </div>
            <h3 class="font-teko mt-30">
              Redes sociais
            </h3>
            <div class="d-flex mt-10 pl-10">
              <a href="http://" target="_blank" rel="noopener noreferrer">
                <i class="fab fs-25 text-roxo fa-twitter" />
              </a>
              <a href="http://" target="_blank" class="mx-15" rel="noopener noreferrer">
                <i class="fab fs-25 text-roxo fa-facebook" />
              </a>
              <a href="http://" target="_blank" rel="noopener noreferrer">
                <i class="fab fs-25 text-roxo fa-youtube" />
              </a>
              <a href="http://" target="_blank" class="mx-15" rel="noopener noreferrer">
                <i class="fab fs-25 text-roxo fa-pinterest" />
              </a>
              <a href="http://" target="_blank" rel="noopener noreferrer">
                <i class="fab fs-25 text-roxo fa-instagram" />
              </a>
            </div>
            <h3 class="font-teko mt-30">
              Telefones
            </h3>
            <div class="d-flex">
              <div class="pl-10 mt-10">
                <h6 class="text-center fs-15 mb-0 mt-20 fw-600">
                  Baln. Camboriú
                </h6>
                <div class="d-flex justify-content-center">
                  <a href="tel:4732400934" class="text-center text-dark">
                    <ion-icon class="text-roxo-escuro fs-23" name="call-outline" style="margin-bottom: -4px; margin-left: -7px; margin-right: 2px;" />+55 (47) 3240-0934
                  </a>
                </div>
                <h6 class="text-center fs-15 mb-0 mt-10 fw-600">
                  Florianópolis
                </h6>
                <div class="d-flex justify-content-center">
                  <a href="tel:4840429661" class="text-center text-dark">
                    <ion-icon class="text-roxo-escuro fs-23" name="call-outline" style="margin-bottom: -4px; margin-left: -7px; margin-right: 2px;" />+55 (48) 4042-9661
                  </a>
                </div>
                <h6 class="text-center fs-15 mb-0 mt-10 fw-600">
                  Curitiba
                </h6>
                <div class="d-flex justify-content-center">
                  <a href="tel:4140427365" class="text-center text-dark">
                    <ion-icon class="text-roxo-escuro fs-23" name="call-outline" style="margin-bottom: -4px; margin-left: -7px; margin-right: 2px;" />+55 (41) 4042-7365
                  </a>
                </div>
                <h6 class="text-center fs-15 mb-0 mt-10 fw-600">
                  Lages
                </h6>
                <div class="d-flex justify-content-center">
                  <a href="tel:4932400948" class="text-center text-dark">
                    <ion-icon class="text-roxo-escuro fs-23" name="call-outline" style="margin-bottom: -4px; margin-left: -7px; margin-right: 2px;" />+55 (49) 3240-0948
                  </a>
                </div>
              </div>
            </div>
          </div>
        </b-collapse>
      </nav>
      <nav v-scroll="ScrollNav" class="navbar d-xs-none d-sm-none d-lg-flex fixed-top nav" :class="{'bg-nav-scroll border-bottom py-10 shadow': NavScroll, 'pt-40': !NavScroll}">
        <div class="container">
          <a href="https://detetivegraziella.com.br" :class="{'text-white': !NavScroll, 'text-grafite': NavScroll}">
            <img v-show="!NavScroll" src="../assets/img/logo-grazi.webp" width="100" alt="Logo Graziela Detetives">
            <img v-show="NavScroll" src="../assets/img/logo-chapeu.webp" width="50" alt="Logo Graziela Detetives">
          </a>
          <div class="ml-auto d-flex">
            <button
              :class="{'text-white': !NavScroll, 'text-grafite': NavScroll}"
              class="btn nav-link d-flex position-relative px-0"
              @click.prevent="$router.push('/')"
            >
              Início
              <i id="arrow-marcacao" class="fs-13 fa fa-arrow-right text-roxo" style="margin-top: 6px;" />
            </button>
            <button
              :class="{'text-white': !NavScroll, 'text-grafite': NavScroll}"
              class="btn nav-link d-flex position-relative px-0 mx-35"
              @click.prevent="$router.push('/sobre/')"
            >
              Sobre
              <i id="arrow-marcacao" class="fs-13 fa fa-arrow-right text-roxo" style="margin-top: 6px;" />
            </button>
            <button
              :class="{'text-white': !NavScroll, 'text-grafite': NavScroll}"
              class="btn nav-link d-flex justify-content-center position-relative px-0"
              @mouseenter="ShowDropdownservicos = true"
              @mouseleave="ShowDropdownservicos = false"
            >
              Serviços
              <transition enter-active-class="animate__animated animate__fadeIn" leave-active-class="animate__animated animate__fadeOut">
                <div v-show="ShowDropdownservicos" class="dropwdown-servicos pt-20">
                  <div class="bg-light position-relative py-10 px-1 cursor-normal d-flex row mx-auto shadow justify-content-center">
                    <div class="seta-dropdown" />
                    <button class="py-1 btn d-flex col-12 fw-500 align-items-center" @click.prevent="$router.push('/servicos/')">
                      Todos os serviços <i class="fa fa-arrow-right ml-2 fs-13 text-roxo" />
                    </button>
                    <button class="py-1 btn d-flex col-12 fw-500 align-items-center" @click.prevent="$router.push('/servicos/investigacao-conjugal/')">
                      Investigação conjugal <i class="fa fa-arrow-right ml-2 fs-13 text-roxo" />
                    </button>
                    <button class="py-1 btn d-flex col-12 fw-500 align-items-center" @click.prevent="$router.push('/servicos/investigacao-empresarial/')">
                      Investigação empresarial <i class="fa fa-arrow-right ml-2 fs-13 text-roxo" />
                    </button>
                    <button class="py-1 btn d-flex col-12 fw-500 align-items-center" @click.prevent="$router.push('/servicos/comportamento-de-filhos/')">
                      Comportamento de filhos <i class="fa fa-arrow-right ml-2 fs-13 text-roxo" />
                    </button>
                    <button class="py-1 btn d-flex col-12 fw-500 align-items-center" @click.prevent="$router.push('/servicos/localizacao-de-pessoas/')">
                      Localização de pessoas <i class="fa fa-arrow-right ml-2 fs-13 text-roxo" />
                    </button>
                    <button class="py-1 btn d-flex col-12 fw-500 align-items-center" @click.prevent="$router.push('/servicos/provas-para-advogados/')">
                      Provas para advogados <i class="fa fa-arrow-right ml-2 fs-13 text-roxo" />
                    </button>
                    <button class="py-1 btn d-flex col-12 fw-500 align-items-center" @click.prevent="$router.push('/servicos/celular-VIP/')">
                      Celular VIP <i class="fa fa-arrow-right ml-2 fs-13 text-roxo" />
                    </button>
                  </div>
                </div>
              </transition>
            </button>
            <button
              :class="{'text-white': !NavScroll, 'text-grafite': NavScroll}"
              class="btn nav-link d-flex justify-content-center position-relative px-0 mx-35"
              @mouseenter="ShowDropdownLocalidades = true"
              @mouseleave="ShowDropdownLocalidades = false"
            >
              Onde atendemos
              <transition enter-active-class="animate__animated animate__fadeIn" leave-active-class="animate__animated animate__fadeOut">
                <div v-show="ShowDropdownLocalidades" class="dropwdown-localidades pt-20">
                  <div class="bg-light position-relative py-10 px-1 cursor-normal d-flex row mx-auto shadow justify-content-center">
                    <div class="seta-dropdown" />
                    <button class="py-1 btn d-flex col-12 fw-500 align-items-center" @click.prevent="$router.push('/detetive-particular-em-Santa-Catarina/')">
                      <i class="fa fa-map-marker-alt mr-2 fs-13 text-roxo" /> Santa Catarina
                    </button>
                    <button class="py-1 btn d-flex col-12 fw-500 align-items-center" @click.prevent="$router.push('/detetive-particular-no-Parana/')">
                      <i class="fa fa-map-marker-alt mr-2 fs-13 text-roxo" /> Paraná
                    </button>
                    <button class="py-1 btn d-flex col-12 fw-500 align-items-center" @click.prevent="$router.push('/detetive-particular-no-Rio-Grande-do-Sul/')">
                      <i class="fa fa-map-marker-alt mr-2 fs-13 text-roxo" /> Rio Grande do Sul
                    </button>
                    <button class="py-1 btn d-flex col-12 fw-500 align-items-center" @click.prevent="$router.push('/detetive-particular-em-Sao-Paulo/')">
                      <i class="fa fa-map-marker-alt mr-2 fs-13 text-roxo" /> São Paulo
                    </button>
                    <button class="py-1 btn d-flex col-12 fw-500 align-items-center" @click.prevent="$router.push('/detetive-particular-no-Rio-de-Janeiro/')">
                      <i class="fa fa-map-marker-alt mr-2 fs-13 text-roxo" /> Rio de Janeiro
                    </button>
                    <button class="py-1 btn d-flex col-12 fw-500 align-items-center" @click.prevent="$router.push('/detetive-particular-no-Distrito-Federal/')">
                      <i class="fa fa-map-marker-alt mr-2 fs-13 text-roxo" /> Distrito Federal
                    </button>
                    <button class="py-1 btn d-flex col-12 fw-500 align-items-center" @click.prevent="$router.push('/detetive-particular-em-Minas-Gerais/')">
                      <i class="fa fa-map-marker-alt mr-2 fs-13 text-roxo" /> Minas Gerais
                    </button>
                    <button class="py-1 btn d-flex col-12 fw-500 align-items-center" @click.prevent="$router.push('/detetive-particular-no-Mato-Grosso-do-Sul/')">
                      <i class="fa fa-map-marker-alt mr-2 fs-13 text-roxo" /> Mato Grosso do Sul
                    </button>
                    <button class="py-1 btn d-flex col-12 fw-500 align-items-center" @click.prevent="$router.push('/detetive-particular-em-Goias/')">
                      <i class="fa fa-map-marker-alt mr-2 fs-13 text-roxo" /> Goiás
                    </button>
                  </div>
                </div>
              </transition>
            </button>
            <button
              :class="{'text-white': !NavScroll, 'text-grafite': NavScroll}"
              class="btn nav-link d-flex mr-35 position-relative px-0"
              @click.prevent="$router.push('/imprensa/')"
            >
              Imprensa
              <i id="arrow-marcacao" class="fs-13 fa fa-arrow-right text-roxo" style="margin-top: 6px;" />
            </button>
            <button
              :class="{'text-white': !NavScroll, 'text-grafite': NavScroll}"
              class="btn nav-link d-flex position-relative px-0"
              @click.prevent="ScrollContato"
            >
              Fale conosco
              <i id="arrow-marcacao" class="fs-13 fa fa-arrow-right text-roxo" style="margin-top: 6px;" />
            </button>
          </div>
        </div>
      </nav>
    </header>
  </div>
</template>
<script>
export default {
  data () {
    return {
      NavScroll: false,
      ShowDropdownservicos: false,
      ShowDropdownLocalidades: false,
      CollapseNav: false,
      IconTimes: false,
      IconBar: true,
      Quantidade_retira_hash: 0
    }
  },
  mounted () {
    this.$root.$on('bv::collapse::state', (collapseId, isJustShown) => {
      if (collapseId === 'collapse-navbar' && isJustShown === true) {
        this.ShowIconTimes()
        document.body.classList.add('overflow-hidden')
        this.CollapseNav = true
        this.NavScroll = true
      }
      if (collapseId === 'collapse-navbar' && isJustShown === false) {
        this.ShowIconBar()
        document.body.classList.remove('overflow-hidden')
        this.CollapseNav = false
        if (window.scrollY < 1) {
          this.NavScroll = false
        }
      }
    })
  },
  methods: {
    ScrollNav () {
      if (window.scrollY > 1) {
        this.NavScroll = true
      } else {
        this.NavScroll = false
      }
    },
    ShowIconTimes () {
      this.IconTimes = true
      this.IconBar = false
    },
    ShowIconBar () {
      this.IconTimes = false
      this.IconBar = true
    },
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
  .animate__animated{
    animation-duration: .3s !important;
    -o-animation-duration: .3s !important;
    -moz-animation-duration: .3s !important;
    -webkit-animation-duration: .3s !important;
  }
  .nav-event{
    height: calc(100vh - 77px);
    overflow-y: scroll;
  }
  nav, nav .container{
    transition: all .3s;
    -o-transition: all .3s;
    -moz-transition: all .3s;
    -webkit-transition: all .3s;
  }
  button.nav-link i#arrow-marcacao{
    width: 0px;
    overflow: hidden;
    transition: all .2s;
    -o-transition: all .2s;
    -moz-transition: all .2s;
    -webkit-transition: all .2s;
  }
  button.nav-link:hover i#arrow-marcacao {
    width: 22px;
    padding-left: 10px;
  }
  .nav-link{
    font-weight: 500;
    letter-spacing: 0.5px;
  }
  .dropwdown-servicos button{
    transform: translateX(0px);
    -o-transform: translateX(0px);
    -moz-transform: translateX(0px);
    -webkit-transform: translateX(0px);
    transition: all .1s;
    -o-transition: all .1s;
    -moz-transition: all .1s;
    -webkit-transition: all .1s;
  }
  .dropwdown-servicos button:hover{
    transform: translateX(7px);
    -o-transform: translateX(7px);
    -moz-transform: translateX(7px);
    -webkit-transform: translateX(7px);
  }
  .dropwdown-localidades button{
    transform: translateX(0px);
    -o-transform: translateX(0px);
    -moz-transform: translateX(0px);
    -webkit-transform: translateX(0px);
    transition: all .1s;
    -o-transition: all .1s;
    -moz-transition: all .1s;
    -webkit-transition: all .1s;
  }
  .dropwdown-localidades button:hover{
    transform: translateX(7px);
    -o-transform: translateX(7px);
    -moz-transform: translateX(7px);
    -webkit-transform: translateX(7px);
  }
  .dropwdown-servicos{
    position: absolute;
    top: 31px;
    width: 280px;
  }
  .dropwdown-localidades{
    position: absolute;
    top: 31px;
    width: 230px;
  }
  .seta-dropdown{
    position: absolute;
    top: -8px;
    height: 16px;
    width: 16px;
    z-index: -1;
    transform: rotate(45deg);
    -o-transform: rotate(45deg);
    -moz-transform: rotate(45deg);
    -webkit-transform: rotate(45deg);
    background-color: var(--roxo_escuro);
  }
  .text-white{
    color: var(--white) !important;
  }
  .bg-nav-scroll{
    background-color: var(--light);
  }
  .marcacao-nav{
    position: absolute;
    bottom: 5px;
    width: 100%;
    height: 2px;
    background-color: var(--roxo_escuro);
    transition: all .3s;
    transform: translateY(5px);
    -o-transform: translateY(5px);
    -moz-transform: translateY(5px);
    -webkit-transform: translateY(5px);
    opacity: 0;
  }
  .nav-link:hover .marcacao-nav{
    transform: translateY(0px);
    -o-transform: translateY(0px);
    -moz-transform: translateY(0px);
    -webkit-transform: translateY(0px);
    opacity: 1;
  }
</style>
