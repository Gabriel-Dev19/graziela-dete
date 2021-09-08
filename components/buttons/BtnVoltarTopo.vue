<template>
  <div>
    <transition enter-active-class="animate__animated animate__fadeIn" leave-active-class="animate__animated animate__fadeOut">
      <div v-show="ShowBtn" v-scroll="ScrollShow">
        <button :class="{'subir-topo': SubirWhatsapp}" class="btn-topo bg-roxo-super-escuro btn shadow d-flex justify-content-center align-items-center" @click="ScrollTop">
          <i class="fa fa-angle-up text-white fs-43 fw-300 mb-1" />
        </button>
      </div>
    </transition>
  </div>
</template>
<script>
export default {
  data () {
    return {
      Quantidade_retira_hash: 0,
      ShowBtn: false,
      SubirWhatsapp: false
    }
  },
  created () {
    if (!this.getGDPR() === true) {
      this.SubirWhatsapp = true
    }

    this.$root.$on('DescerTopo', () => {
      this.SubirWhatsapp = false
    })
  },
  methods: {
    ScrollShow () {
      if (window.scrollY > 700) {
        this.ShowBtn = true
      } else {
        this.ShowBtn = false
      }
    },
    getGDPR () {
      if (process.browser) {
        return localStorage.getItem('GDPR:accepted', true)
      }
    },
    ScrollTop () {
      this.$smoothScroll({
        scrollTo: document.body,
        duration: 500,
        offset: 0
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
  @media (min-width: 1px) {
    .btn-topo{
      position: fixed;
      bottom: 15px;
      left: 15px;
      width: 48px;
      height: 48px;
      z-index: 1000;
      border-radius: 50%;
    }
    .subir-topo{
      bottom: 220px !important;
      z-index: 1030 !important;
    }
  }
  @media (min-width: 576px) {
    .btn-topo{
      position: fixed;
      bottom: 30px;
      left: 30px;
      width: 48px;
      height: 48px;
      z-index: 1000;
      border-radius: 50%;
    }
    .subir-topo{
      bottom: 180px !important;
      z-index: 1030 !important;
    }
  }
  @media (min-width: 768px) {
    .subir-topo{
      bottom: 150px !important;
      z-index: 1030 !important;
    }
  }
  @media (min-width: 1200px) {
    .subir-topo{
      bottom: 100px !important;
      z-index: 1030 !important;
    }
  }
</style>
