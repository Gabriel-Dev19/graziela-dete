<template>
  <div>
    <Navbar />
    <Home />
    <section class="height-100-vh" />
  </div>
</template>

<script>
import Home from '~/components/Home.vue'
import Navbar from '~/components/Navbar.vue'
export default {
  components: { Navbar, Home }
}
</script>
