<template>
  <div>
    <Home title-home="Serviços de detetive particular" :bg-home="true" />
    <section class="height-100-vh" />
  </div>
</template>

<script>
import Home from '~/components/Home.vue'
export default {
  components: { Home },
  layout: 'LayoutServicos'
}
</script>
