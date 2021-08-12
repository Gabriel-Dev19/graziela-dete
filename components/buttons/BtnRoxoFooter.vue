<template>
  <button class="btn btn-roxo shadow-sm border-radius-0 px-20 fw-500" @click.prevent="ScrollFooter">
    {{ nameBtn }}
  </button>
</template>
<script>
export default {
  props: {
    nameBtn: {
      type: String,
      default: 'Fale com a Grazi'
    }
  },
  data () {
    return {
      Quantidade_retira_hash: 0
    }
  },
  methods: {
    ScrollFooter () {
      this.$smoothScroll({
        scrollTo: document.getElementById('footer'),
        duration: 500,
        offset: -100
      })
      setTimeout(() => {
        this.HideHash()
      }, 490)
      this.$root.$emit('PulseFooter')
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
