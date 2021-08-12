<template>
  <div class="pt-100">
    <div class="container">
      <h1 class="font-teko position-relative d-flex justify-content-center text-uppercase text-center">
        Detetives altamente capacitados
        <div class="separation-tema" />
      </h1>
      <div class="d-flex mt-120 row mx-auto">
        <div class="col-lg px-0">
          <span class="display-3 d-block fw-500 font-teko">01.</span>
          <h4 class="text-uppercase font-teko mt-30">
            Diagnóstico
          </h4>
          <p class="mt-2 fw-500 fs-15">
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Modi soluta, voluptatibus totam sed temporibus
            consequatur, facilis, fuga nihil delectus quas voluptatem praesentium odio. Id ducimus fuga corporis vel sunt aliquid.
          </p>
          <div class="detalhe-bottom mt-20">
            <div class="h-100 bg-roxo-escuro" />
          </div>
          <button class="btn text-uppercase mt-2 px-0 fs-20 d-flex align-items-center fw-500 btn-teko" @click.prevent="ScrollContato">
            Faça um diagnóstico <i class="fa fa-angle-right fw-600 ml-1 mb-1" />
          </button>
        </div>
        <div class="col-lg px-0 my-xs-90 my-sm-90 my-lg-0 mx-lg-50">
          <span class="display-3 d-block fw-500 font-teko">02.</span>
          <h4 class="text-uppercase font-teko mt-30">
            Planejamento
          </h4>
          <p class="mt-2 fw-500 fs-15">
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Modi soluta, voluptatibus totam sed temporibus
            consequatur, facilis, fuga nihil delectus quas voluptatem praesentium odio. Id ducimus fuga corporis vel sunt aliquid.
          </p>
          <div class="detalhe-bottom mt-20">
            <div class="h-100 bg-roxo-escuro" />
          </div>
          <button class="btn text-uppercase mt-2 px-0 fs-20 d-flex align-items-center fw-500 btn-teko" @click.prevent="ScrollContato">
            Planeje com a gente <i class="fa fa-angle-right fw-600 ml-1 mb-1" />
          </button>
        </div>
        <div class="col-lg px-0">
          <span class="display-3 d-block fw-500 font-teko">03.</span>
          <h4 class="text-uppercase font-teko mt-30">
            Investigação
          </h4>
          <p class="mt-2 fw-500 fs-15">
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Modi soluta, voluptatibus totam sed temporibus
            consequatur, facilis, fuga nihil delectus quas voluptatem praesentium odio. Id ducimus fuga corporis vel sunt aliquid.
          </p>
          <div class="detalhe-bottom mt-20">
            <div class="h-100 bg-roxo-escuro" />
          </div>
          <button class="btn text-uppercase mt-2 px-0 fs-20 d-flex align-items-center fw-500 btn-teko" @click.prevent="ScrollContato">
            Saiba de tudo! <i class="fa fa-angle-right fw-600 ml-1 mb-1" />
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
  .detalhe-bottom div{
    transition: all .3s;
    -o-transition: all .3s;
    -moz-transition: all .3s;
    -webkit-transition: all .3s;
  }
  span.display-3{
    line-height: 0px;
  }
  .detalhe-bottom{
    height: 2px;
    width: 100%;
    background-color: #d5d5d5;
  }
  .detalhe-bottom div{
    width: 0%;
  }
  .col-lg:hover .detalhe-bottom div{
    width: 100%;
  }
  .separation-tema{
    position: absolute;
    height: 3px;
    width: 200px;
    bottom: -10px;
    border-radius: 3px;
    background-color: var(--roxo);
  }
</style>
