<template>
  <div>
    <Navbar />
    <Home title-home="Sessão de imprensa - Entrevistas" :bg-imprensa="true" />
    <section id="imprensa" class="pt-100">
      <div class="container">
        <h1 class="font-teko position-relative col-12 px-0 d-flex justify-content-center text-uppercase text-center">
          Veja todas as entrevistas de  Graziella
          <div class="separation-tema" />
        </h1>
        <nav class="navbar py-0 nav justify-content-center mt-40">
          <NuxtLink to="/imprensa/" class="fs-18 mx-3 mt-3 text-grafite no-underline fw-500">
            <ion-icon name="apps-outline" style="margin-bottom: -3px" /> Todas
          </NuxtLink>
          <NuxtLink to="/imprensa/radio/" class="fs-18 mx-3 mt-3 text-grafite no-underline fw-500">
            <ion-icon name="radio-outline" style="margin-bottom: -3px" /> Rádio
          </NuxtLink>
          <NuxtLink to="/imprensa/televisao/" class="fs-18 mx-3 mt-3 text-grafite no-underline fw-500">
            <ion-icon name="tv-outline" style="margin-bottom: -3px" /> Televisão
          </NuxtLink>
          <NuxtLink to="/imprensa/revista/" class="fs-18 mx-3 mt-3 text-grafite no-underline fw-500">
            <ion-icon name="book-outline" style="margin-bottom: -3px" /> Revistas
          </NuxtLink>
          <NuxtLink to="/imprensa/jornal/" class="fs-18 mx-3 mt-3 text-grafite no-underline fw-500">
            <ion-icon name="newspaper-outline" style="margin-bottom: -3px" /> Jornais
          </NuxtLink>
          <NuxtLink to="/imprensa/fotos/" class="fs-18 mx-3 mt-3 text-grafite no-underline fw-500">
            <ion-icon name="images-outline" style="margin-bottom: -3px" /> Fotos
          </NuxtLink>
        </nav>
        <Nuxt />
      </div>
    </section>
    <Servicos class="mt-150" />
    <ParalaxHome />
    <Numeros />
    <Contato />
    <Footer />
    <ModalWhatsapp />
    <BtnVoltarTopo />
  </div>
</template>
<script>
import Vue from '../node_modules/vue'
import Navbar from '../components/Navbar.vue'
import VueSmoothScroll from '../node_modules/vue2-smooth-scroll'
import BtnVoltarTopo from '~/components/buttons/BtnVoltarTopo.vue'
import Contato from '~/components/Contato.vue'
import Footer from '~/components/Footer.vue'
import Numeros from '~/components/Numeros.vue'
import ParalaxHome from '~/components/ParalaxHome.vue'
import Servicos from '~/components/Servicos.vue'
import Home from '~/components/Home.vue'
import ModalWhatsapp from '~/components/ModalWhatsapp.vue'
Vue.use(VueSmoothScroll)
Vue.directive('scroll', {
  inserted (el, binding) {
    const f = function (evt) {
      if (binding.value(evt, el)) {
        window.removeEventListener('scroll', f)
      }
    }
    window.addEventListener('scroll', f)
  }
})
export default {
  components: {
    Navbar,
    BtnVoltarTopo,
    Servicos,
    ParalaxHome,
    Numeros,
    Contato,
    Footer,
    Home,
    ModalWhatsapp
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
    background-color: var(--roxo);
  }
  .borda-tema-fina{
    position: absolute;
    height: 2px;
    width: 200px;
    bottom: -1px;
    border-radius: 3px;
    background-color: var(--roxo);
  }
  a.text-grafite{
    color: var(--grafite) !important;
    border-bottom: 2px solid transparent;
  }
  a.nuxt-link-exact-active {
    transition: all .5s;
    -o-transition: all .5s;
    -moz-transition: all .5s;
    -webkit-transition: all .5s;
    border-bottom: 2px solid var(--roxo_escuro);
  }
</style>
