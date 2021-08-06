<template>
  <div>
    <Navbar />
    <Home bg-home="true" />
    <Planejamento />
    <Servicos />
    <ParalaxHome />
    <Numeros />
    <Motivos />
    <Comentarios />
    <section class="height-100-vh" />
  </div>
</template>

<script>
import Home from '~/components/Home.vue'
import Navbar from '~/components/Navbar.vue'
import Planejamento from '~/components/Planejamento.vue'
import Servicos from '~/components/Servicos.vue'
import ParalaxHome from '~/components/ParalaxHome.vue'
import Numeros from '~/components/Numeros.vue'
import Motivos from '~/components/Motivos.vue'
import Comentarios from '~/components/Comentarios.vue'
export default {
  components: {
    Navbar,
    Home,
    Planejamento,
    Servicos,
    ParalaxHome,
    Numeros,
    Motivos,
    Comentarios
  }
}
</script>
