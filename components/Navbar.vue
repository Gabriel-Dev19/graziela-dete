<template>
  <div>
    <header>
      <nav v-scroll="ScrollNav" class="navbar align-items-center d-lg-none fixed-top nav" :class="{'bg-roxo-escuro shadow': NavScroll, 'pt-40': !NavScroll}">
        <div class="container">
          <a href="" class="text-white">
            Logo
          </a>
          <button class="btn py-0 px-0">
            <ion-icon class="text-white fs-40" name="menu-outline" style="margin-bottom: -7px;" />
          </button>
        </div>
      </nav>
      <nav v-scroll="ScrollNav" class="navbar d-xs-none d-sm-none d-lg-flex fixed-top nav" :class="{'bg-roxo-escuro shadow': NavScroll, 'pt-40': !NavScroll}">
        <div class="container">
          <a href="" class="text-white">
            Logo
          </a>
          <div class="ml-auto d-flex">
            <button class="btn nav-link position-relative px-0" :class="{'text-white': NavScroll}" @click.prevent="$router.push('/')">
              Início
              <div class="marcacao-nav" :class="{'bg-white': NavScroll, 'bg-roxo': !NavScroll}" />
            </button>
            <button class="btn nav-link position-relative px-0 mx-35" :class="{'text-white': NavScroll}" @click.prevent="$router.push('/sobre')">
              Sobre
              <div class="marcacao-nav" :class="{'bg-white': NavScroll, 'bg-roxo': !NavScroll}" />
            </button>
            <button class="btn nav-link position-relative px-0" :class="{'text-white': NavScroll}" @click.prevent="$router.push('/servicos')">
              Serviços
              <div class="marcacao-nav" :class="{'bg-white': NavScroll, 'bg-roxo': !NavScroll}" />
            </button>
            <button class="btn nav-link position-relative px-0 mx-35" :class="{'text-white': NavScroll}">
              Onde atendemos
              <div class="marcacao-nav" :class="{'bg-white': NavScroll, 'bg-roxo': !NavScroll}" />
            </button>
            <button class="btn nav-link position-relative px-0" :class="{'text-white': NavScroll}">
              Fale conosco
              <div class="marcacao-nav" :class="{'bg-white': NavScroll, 'bg-roxo': !NavScroll}" />
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
      NavScroll: false
    }
  },
  methods: {
    ScrollNav () {
      if (window.scrollY > 1) {
        this.NavScroll = true
      } else {
        this.NavScroll = false
      }
    }
  }
}
</script>
<style scoped>
  nav{
    transition: all .3s;
    -o-transition: all .3s;
    -moz-transition: all .3s;
    -webkit-transition: all .3s;
  }
  .nav-link{
    color: var(--white);
    font-weight: 500;
    letter-spacing: 0.5px;
  }
  .text-white{
    color: var(--white) !important;
  }
  .marcacao-nav{
    position: absolute;
    bottom: 5px;
    width: 100%;
    height: 2px;
    background-color: var(--roxo);
    transition: all .3s;
    transform: translateY(5px);
    opacity: 0;
  }
  .nav-link:hover .marcacao-nav{
    transform: translateY(0px);
    opacity: 1;
  }
  .nav-link:hover{
    color: var(--roxo_claro);
  }
</style>
