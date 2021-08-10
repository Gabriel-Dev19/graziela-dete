<template>
  <div>
    <Home title-home="Sobre a agência Graziela Bastos" :bg-home="true" />
    <section class="height-100-vh" />
  </div>
</template>

<script>
import Home from '~/components/Home.vue'
export default {
  components: { Home },
  layout: 'LayoutSobre'
}
</script>
