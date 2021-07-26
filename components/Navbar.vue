<template>
  <div>
    <header>
      <nav class="navbar d-lg-none fixed-top pt-30 nav">
        <div class="container">
          <a href="">
            <img src="" alt="Logo Graziela">
          </a>
          <button class="btn">
            <ion-icon class="text-white fs-40" name="menu-outline" />
          </button>
        </div>
      </nav>
      <nav class="navbar d-xs-none d-sm-none d-lg-flex fixed-top pt-30 nav">
        <div class="container">
          <a href="">
            <img src="" alt="Logo Graziela">
          </a>
          <div class="ml-auto d-flex">
            <button class="btn nav-link position-relative px-0">
              Home
              <div class="marcacao-nav" />
            </button>
            <button class="btn nav-link position-relative px-0 mx-35">
              Sobre
              <div class="marcacao-nav" />
            </button>
            <button class="btn nav-link position-relative px-0">
              Serviços
              <div class="marcacao-nav" />
            </button>
            <button class="btn nav-link position-relative px-0 mx-35">
              Onde atendemos
              <div class="marcacao-nav" />
            </button>
            <button class="btn nav-link position-relative px-0">
              Fale comigo
              <div class="marcacao-nav" />
            </button>
          </div>
        </div>
      </nav>
    </header>
  </div>
</template>
<script>
export default {

}
</script>
<style scoped>
  .nav-link{
    color: var(--white);
    font-size: 15px;
    font-weight: 500;
    letter-spacing: 0.5px;
  }
  .marcacao-nav{
    position: absolute;
    bottom: 4px;
    width: 100%;
    height: 2px;
    background-color: var(--roxo);
    transition: all .3s;
    transform: translateY(5px);
    opacity: 0;
  }
  .nav-link:hover .marcacao-nav{
    transform: translateY(0px);
    opacity: 1;
  }
  .nav-link:hover{
    color: var(--roxo_claro);
  }
</style>
