<template>
  <Nuxt />
</template>
<script>
import Vue from '../node_modules/vue'
Vue.directive('scroll', {
  inserted (el, binding) {
    const f = function (evt) {
      if (binding.value(evt, el)) {
        window.removeEventListener('scroll', f)
      }
    }
    window.addEventListener('scroll', f)
  }
})
export default {

}
</script>
