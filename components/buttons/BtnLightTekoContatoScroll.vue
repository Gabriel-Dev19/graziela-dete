<template>
  <button class="btn font-teko text-uppercase d-flex align-items-center fs-21 pl-20 pb-1 fw-500 border-radius-0 btn-light" @click.prevent="ScrollContato">
    {{ nameBtn }} <i class="fa fa-angle-right fw-500 ml-2 mb-1" />
  </button>
</template>
<script>
export default {
  props: {
    nameBtn: {
      type: String,
      default: 'Contato'
    }
  },
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
        offset: -100
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

</style>
