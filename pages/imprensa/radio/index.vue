<template>
  <div class="d-flex px-3 row max-auto">
    <div class="w-imprensa mt-50">
      <iframe
        class="col-12 shadow-sm px-0"
        src="https://www.youtube.com/embed/cTs6FduQ4A8"
        title="YouTube video player"
        frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
        allowfullscreen
      />
      <h3 class="mt-3 mb-1 font-teko">
        Entrevista completa de Graziella Bastos para a Magia FM 107.3
      </h3>
      <div class="height-2-px bg-roxo-escuro col-12 px-0" />
      <p class="fw-500 mt-10">
        Confira a entrevista completa de Graziella Bastos para a Magia FM 107.3, onde ela explica mais sobre a profissão
        de detetive particular e ensina técnicas para descobrir uma possível infidelidade e o que fazer em casos como esse!
      </p>
    </div>
  </div>
</template>

<script>
export default {
  layout: 'LayoutImprensa',
  head: {
    title: 'Imprensa - Rádio - Agência de detetives Graziella Bastos'
  }
}
</script>
<style scoped>
  h3.font-teko{
    line-height: 29px;
  }
  @media (min-width: 1px) {
    iframe{
      height: 320px;
    }
  }
  @media (min-width: 992px) {
    .w-imprensa{
      width: 32%;
    }
    iframe{
      height: 220px;
    }
  }
</style>
