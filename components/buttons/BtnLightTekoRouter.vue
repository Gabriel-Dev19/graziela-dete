<template>
  <button class="btn font-teko text-uppercase d-flex align-items-center fs-21 pl-20 pb-1 fw-500 border-radius-0 btn-light" @click.prevent="$router.push(routerTo)">
    {{ nameBtn }} <i class="fa fa-angle-right fw-500 ml-2 mb-1" />
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
