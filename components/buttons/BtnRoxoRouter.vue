<template>
  <button class="btn btn-roxo shadow-sm border-radius-0 px-20 fw-500" @click.prevent="$router.push(routerTo)">
    {{ nameBtn }}
  </button>
</template>
<script>
export default {
  props: {
    nameBtn: {
      type: String,
      default: 'Saiba Mais'
    },
    routerTo: {
      type: String,
      default: '/'
    }
  }
}
</script>
<style scoped>

</style>
