<template>
  <div>
    <Home title-home="Detetive particular no Rio Grande do Sul" :bg-home="true" />
    <section class="pt-100">
      <div class="container">
        <h1 class="font-teko position-relative col-12 px-0 d-flex justify-content-center text-uppercase text-center">
          Contate um detetive particular no Rio Grande do Sul
          <div class="separation-tema" />
        </h1>
        <p class="mt-35 text-center fw-500 px-0">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Animi ipsam consequatur modi rem voluptas molestias
          omnis sed iusto veniam error? Nostrum quaerat inventore earum commodi nihil, et ad mollitia voluptatem.
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Animi ipsam consequatur modi rem voluptas molestias
          omnis sed iusto veniam error? Nostrum quaerat inventore earum commodi nihil, et ad mollitia voluptatem.
        </p>
        <div class="d-flex row mx-auto justify-content-center mt-4">
          <btn-roxo-contato-scroll class="col-xs-9" name-btn="Entre em contato" />
          <btn-roxo-footer class="ml-sm-3 mt-xs-2 col-xs-9" />
        </div>
        <h1 class="font-teko d-flex text-center text-uppercase mt-90 justify-content-center position-relative mb-1">
          Confira as cidades atendidas
          <div class="borda-tema-fina" />
        </h1>
      </div>
    </section>
    <section class=" col-12 px-0">
      <div class="container px-xs-0">
        <!-- Cidades A -->
        <div class="position-relative bg-roxo-escuro border shadow border-radius-10 overflow-hidden col-12 mt-30 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-600 mb-1">
              A
            </h5>
          </div>
          <div class="col-lg px-0 mt-4">
            <a class="d-flex col-auto px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="AltoFeliz">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Alto Feliz - RS
            </a>
            <a class="d-flex col-auto px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Alvorada">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Alvorada - RS
            </a>
            <a class="d-flex col-auto px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="AmaralFerrador">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Amaral Ferrador – RS
            </a>
            <a class="d-flex col-auto px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="AntaGorda">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Anta Gorda – RS
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-auto px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Arambare">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Arambaré – RS
            </a>
            <a class="d-flex col-auto px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Ararica">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Araricá – RS
            </a>
            <a class="d-flex col-auto px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="ArroioDoMeio">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Arroio do Meio – RS
            </a>
            <a class="d-flex col-auto px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="ArroioDoSal">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Arroio do Sal – RS
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-auto px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="ArroioDoTigre">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Arroio do Tigre – RS
            </a>
            <a class="d-flex col-auto px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="ArroioDosRatos">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Arroio dos Ratos – RS
            </a>
            <a class="d-flex col-auto px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Arvorezinha">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Arvorezinha – RS
            </a>
          </div>
        </div>
        <!-- Cidades B -->
        <div class="position-relative bg-roxo-escuro border shadow border-radius-10 mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-600 mb-0">
              B
            </h5>
          </div>
          <div class="col-lg px-0 mt-4">
            <a class="d-flex col-12 px-0 py-0 mt-1 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="BalnearioPinhal">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Balneário Pinhal - RS
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Barao">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Barão - RS
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="BaraoDoTriunfo">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Barão do Triunfo – RS
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="BomRetiroDoSul">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Bom Retiro do Sul – RS
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="BoqueirãoDoLeao">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Boqueirão do Leão – RS
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="BomPrincipio">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Bom Princípio – RS
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Brochier">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Brochier – RS
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Butiá">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Butiá – RS
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="BarraDoRibeiro">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Barra do Ribeiro – RS
            </a>
          </div>
        </div>
        <!-- Cidades C -->
        <div class="position-relative bg-roxo-escuro border shadow border-radius-10 mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-600 mb-0">
              C
            </h5>
          </div>
          <div class="col-lg px-0 mt-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="CachoeiraDoSul">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Cachoeira do Sul – RS
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Cachoeirinha">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Cachoeirinha – RS
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Camaqua">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Camaquã – RS
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="CampoBom">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Campo Bom – RS
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="CerroBranco">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Cerro Branco – RS
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="CerroGrandeDoSul">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Cerro Grande do Sul – RS
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Charqueadas">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Charqueadas – RS
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Candelaria">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Candelária – RS
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Canoas">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Canoas – RS
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="CanudosDoVale">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Canudos do Vale – RS
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="CapaoDaCanoa">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Capão da Canoa – RS
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Chuvisca">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Chuvisca – RS
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Cidreira">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Cidreira – RS
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Colinas">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Colinas – RS
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="CapelaDeSantana">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Capela de Santana – RS
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Capitao">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Capitão – RS
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="CapivariDoSul">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Capivari do Sul – RS
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Caraa">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Caraá – RS
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="CoqueiroBaixo">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Coqueiro Baixo – RS
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Cristal">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Cristal – RS
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="CruzeiroDoSul">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Cruzeiro do Sul – RS
            </a>
          </div>
        </div>
        <!-- Cidades D -->
        <div class="position-relative bg-roxo-escuro border shadow border-radius-10 mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-600 mb-0">
              D
            </h5>
          </div>
          <div class="col-lg mt-4 px-0">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="DoisIrmaos">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Dois Irmãos – RS
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="DomFeliciano">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Dom Feliciano – RS
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="DomPedroDeAlcantara">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Dom Pedro de Alcântara – RS
            </a>
          </div>
        </div>
        <!-- Cidades E -->
        <div class="position-relative bg-roxo-escuro border shadow border-radius-10 mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-600 mb-0">
              E
            </h5>
          </div>
          <a class="d-flex col-12 mt-4 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="EldoradoDoSul">
            <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Eldorado do Sul – RS
          </a>
          <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Esteio">
            <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Esteio – RS
          </a>
          <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Estrela">
            <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Estrela – RS
          </a>
        </div>
        <!-- Cidades F -->
        <div class="position-relative bg-roxo-escuro border shadow border-radius-10 mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-600 mb-0">
              F
            </h5>
          </div>
          <a class="d-flex col-12 mt-4 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="FazendaVilanova">
            <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Fazenda Vilanova – RS
          </a>
          <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Feliz">
            <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Feliz – RS
          </a>
        </div>
        <!-- Cidades G -->
        <div class="position-relative bg-roxo-escuro border shadow border-radius-10 mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-600 mb-0">
              G
            </h5>
          </div>
          <div class="col-lg px-0 mt-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="GeneralCamara">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> General Câmara – RS
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Glorinha">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Glorinha – RS
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Gravatai">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Gravataí – RS
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Guaiba">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Guaíba – RS
            </a>
          </div>
        </div>
        <!-- Cidades H -->
        <div class="position-relative bg-roxo-escuro border shadow border-radius-10 mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-600 mb-0">
              H
            </h5>
          </div>
          <a class="d-flex col-12 px-0 mt-4 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Harmonia">
            <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Harmonia – RS
          </a>
        </div>
        <!-- Cidades I -->
        <div class="position-relative bg-roxo-escuro border shadow border-radius-10 mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-600 mb-0">
              I
            </h5>
          </div>
          <div class="col-lg px-0 mt-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Ibirama">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Ibirama – RS
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Igrejinha">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Igrejinha – RS
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Ilopolis">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Ilópolis – RS
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Imigrante">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Imigrante – RS
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Itati">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Itati – RS
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Ivoti">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Ivoti – RS
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Imbe">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Imbé – RS
            </a>
          </div>
        </div>
        <!-- Cidades L -->
        <div class="position-relative bg-roxo-escuro border shadow border-radius-10 mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-600 mb-0">
              L
            </h5>
          </div>
          <div class="col-lg px-0 mt-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Lagoao">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Lagoão – RS
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Lajedo">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Lajedo – RS
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="LindolfoCollor">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Lindolfo Collor – RS
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="LinhaNova">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Linha Nova – RS
            </a>
          </div>
        </div>
        <!-- Cidades M -->
        <div class="position-relative bg-roxo-escuro border shadow border-radius-10 mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-600 mb-0">
              M
            </h5>
          </div>
          <div class="col-lg px-0 mt-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Maquine">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Maquiné – RS
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="MarianaPimentel">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Mariana Pimentel – RS
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="MarquesDeSouza">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Marques de Souza – RS
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="MatoLeitao">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Mato Leitão – RS
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="MinasDoLeao">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Minas do Leão – RS
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Montenegro">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Montenegro – RS
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="MorrinhosDoSul">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Morrinhos do Sul – RS
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="MorroReuter">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Morro Reuter – RS
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Mostardas">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Mostardas – RS
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Mucum">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Mucum – RS
            </a>
          </div>
        </div>
        <!-- Cidades N -->
        <div class="position-relative bg-roxo-escuro border shadow border-radius-10 mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-600 mb-0">
              N
            </h5>
          </div>
          <div class="col-lg px-0 mt-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="NovaBrescia">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Nova Bréscia – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="NovaHartz">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Nova Hartz – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="NovaSantaRita">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Nova Santa Rita – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="NovoHamburgo">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Novo Hamburgo – RS
            </a>
          </div>
        </div>
        <!-- Cidades O -->
        <div class="position-relative bg-roxo-escuro border shadow border-radius-10 mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-600 mb-0">
              O
            </h5>
          </div>
          <a class="d-flex col-12 mt-4 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Osorio">
            <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Osório – RS
          </a>
        </div>
        <!-- Cidades P -->
        <div class="position-relative bg-roxo-escuro border shadow border-radius-10 mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-600 mb-0">
              P
            </h5>
          </div>
          <div class="col-lg px-0 mt-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="PalmaresDoSul">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Palmares do Sul – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="PantanoGrande">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Pantano Grande – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="PareciNovo">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Pareci Novo – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Parobe">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Parobé – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="PassoDoSobrado">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Passo do Sobrado – RS
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Paverema">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Paverema – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="PoçoDasAntas">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Poço das Antas – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Portao">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Portão – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="PortoAlegre">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Porto Alegre – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="PousoNovo">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Pouso Novo – RS
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="PresidenteLucena">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Presidente Lucena – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Progresso">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Progresso – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Putinga">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Putinga – RS
            </a>
          </div>
        </div>
        <!-- Cidades R -->
        <div class="position-relative bg-roxo-escuro border shadow border-radius-10 mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-600 mb-0">
              R
            </h5>
          </div>
          <div class="col-lg px-0 mt-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Relvado">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Relvado – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="RioPardo">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Rio Pardo – RS
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="RocaSales">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Roca Sales – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Rolante">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Rolante – RS
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Riozinho">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Riozinho – RS
            </a>
          </div>
        </div>
        <!-- Cidades S -->
        <div class="position-relative bg-roxo-escuro border shadow border-radius-10 mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-600 mb-0">
              S
            </h5>
          </div>
          <div class="col-lg px-0 mt-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="SalvadorDoSul">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Salvador do Sul – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="SantaClaraDoSul">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Santa Clara do Sul - RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="SantaCruzDoSul">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Santa Cruz do Sul - RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="SantaMariaDoHerval">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Santa Maria do Herval - RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="SantoAntonioDaPatrulha">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Santo Antônio da Patrulha - RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="SaoJeronimo">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> São Jerônimo – RS
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="SaoJoseDoHortencio">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> São José do Hortêncio – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="SaoLeopoldo">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> São Leopoldo – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="SaoSebastiaoDoCai">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> São Sebastião do Cai – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="SaoVendelino">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> São Vendelino – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Sapiranga">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Sapiranga – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="SapucaiaDoSul">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Sapucaia do Sul – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Segredo">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Segredo – RS
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="SentinelaDoSul">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Sentinela do Sul – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Serio">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Sério – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="SertaoSantana">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Sertão Santana – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Sinimbu">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Sinimbu – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Sobradinho">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Sobradinho – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="SantanaDoLivramento">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Santana do Livramento – RS
            </a>
          </div>
        </div>
        <!-- Cidades T -->
        <div class="position-relative bg-roxo-escuro border shadow border-radius-10 mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-600 mb-0">
              T
            </h5>
          </div>
          <div class="col-lg px-0 mt-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Tabai">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Tabaí – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Tapes">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Tapes – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Taquara">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Taquara – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Travesseiro">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Travesseiro – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Tunas">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Tunas – RS
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Taquari">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Taquari – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Tavares">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Tavares – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="TerraDeAreia">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Terra de Areia – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="TresCachoeiras">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Três Cachoeiras – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="TresCoroas">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Três Coroas – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Tupandi">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Tupandi – RS
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Teutonia">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Teutônia – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Torres">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Torres – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Tramandai">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Tramandaí – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="TresForquilhas">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Três Forquilhas – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Triunfo">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Triunfo – RS
            </a>
          </div>
        </div>
        <!-- Cidades U -->
        <div class="position-relative bg-roxo-escuro border shadow border-radius-10 mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-600 mb-0">
              U
            </h5>
          </div>
          <a class="d-flex col-12 mt-4 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Uruguaiana">
            <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Uruguaiana – RS
          </a>
        </div>
        <!-- Cidades V -->
        <div class="position-relative bg-roxo-escuro border shadow border-radius-10 mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-600 mb-0">
              V
            </h5>
          </div>
          <div class="col-lg px-0 mt-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="ValeDoSol">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Vale do Sol – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="ValeReal">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Vale Real – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Viamao">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Viamão – RS
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="ValeVerde">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Vale Verde – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="VenancioAires">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Venâncio Aires – RS
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="VeraCruz">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Vera Cruz – RS
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="VespasianoCorreia">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Vespasiano Correia – RS
            </a>
          </div>
        </div>
        <!-- Cidades X -->
        <div class="position-relative bg-roxo-escuro border shadow border-radius-10 mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-600 mb-0">
              X
            </h5>
          </div>
          <a class="d-flex col-12 mt-4 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="XangriLa">
            <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Xangri-Lá – RS
          </a>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import BtnRoxoContatoScroll from '~/components/buttons/BtnRoxoContatoScroll.vue'
import BtnRoxoFooter from '~/components/buttons/BtnRoxoFooter.vue'
import Home from '~/components/Home.vue'
export default {
  components: { Home, BtnRoxoContatoScroll, BtnRoxoFooter },
  layout: 'LayoutSobre',
  head: {
    title: 'Detetive particular no Rio Grande do Sul - Agência de detetives Graziella Bastos'
  },
  mounted () {
    this.$smoothScroll({
      scrollTo: document.body,
      duration: 0,
      offset: 0
    })
    this.HideHash()
  },
  methods: {
    HideHash () {
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
    },
    AltoFeliz () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Alto-Feliz-RS/')
    },
    Alvorada () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Alvorada-RS/')
    },
    AmaralFerrador () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Amaral-Ferrador-RS/')
    },
    AntaGorda () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Anta-Gorda-RS/')
    },
    Arambare () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Arambare-RS/')
    },
    Ararica () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Ararica-RS/')
    },
    ArroioDoMeio () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Arroio-do-Meio-RS/')
    },
    ArroioDoSal () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Arroio-do-Sal-RS/')
    },
    ArroioDoTigre () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Arroio-do-Tigre-RS/')
    },
    ArroioDosRatos () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Arroio-dos-Ratos-RS/')
    },
    Arvorezinha () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Arvorezinha-RS/')
    },
    BalnearioPinhal () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Balneario-Pinhal-RS/')
    },
    Barao () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Barao-RS/')
    },
    BaraoDoTriunfo () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Barao-do-Triunfo-RS/')
    },
    BomRetiroDoSul () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Bom-Retiro-do-Sul-RS/')
    },
    BoqueirãoDoLeao () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Boqueirao-do-Leao-RS/')
    },
    BomPrincipio () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Bom-Principio-RS/')
    },
    Brochier () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Brochier-RS/')
    },
    Butiá () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Butia-RS/')
    },
    BarraDoRibeiro () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Barra-do-Ribeiro-RS/')
    },
    CachoeiraDoSul () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Cachoeira-do-Sul-RS/')
    },
    Cachoeirinha () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Cachoeirinha-RS/')
    },
    Camaqua () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Camaqua-RS/')
    },
    CampoBom () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Campo-Bom-RS/')
    },
    CerroBranco () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Cerro-Branco-RS/')
    },
    CerroGrandeDoSul () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Cerro-Grande-do-Sul-RS/')
    },
    Charqueadas () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Charqueadas-RS/')
    },
    Candelaria () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Candelaria-RS/')
    },
    Canoas () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Canoas-RS/')
    },
    CanudosDoVale () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Canudos-do-Vale-RS/')
    },
    CapaoDaCanoa () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Capao-da-Canoa-RS/')
    },
    Chuvisca () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Chuvisca-RS/')
    },
    Cidreira () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Cidreira-RS/')
    },
    Colinas () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Colinas-RS/')
    },
    CapelaDeSantana () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Capela-de-Santana-RS/')
    },
    Capitao () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Capitao-RS/')
    },
    CapivariDoSul () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Capivari-do-Sul-RS/')
    },
    Caraa () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Caraa-RS/')
    },
    CoqueiroBaixo () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Coqueiro-Baixo-RS/')
    },
    Cristal () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Cristal-RS/')
    },
    CruzeiroDoSul () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Cruzeiro-do-Sul-RS/')
    },
    DoisIrmaos () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Dois-Irmaos-RS/')
    },
    DomFeliciano () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Dom-Feliciano-RS/')
    },
    DomPedroDeAlcantara () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Dom-Pedro-de-Alcantara-RS/')
    },
    EldoradoDoSul () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Eldorado-do-Sul-RS/')
    },
    Esteio () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Esteio-RS/')
    },
    Estrela () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Estrela-RS/')
    },
    FazendaVilanova () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Fazenda-Vilanova-RS/')
    },
    Feliz () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Feliz-RS/')
    },
    GeneralCamara () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-General-Camara-RS/')
    },
    Glorinha () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Glorinha-RS/')
    },
    Gravatai () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Gravatai-RS/')
    },
    Guaiba () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Guaiba-RS/')
    },
    Harmonia () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Harmonia-RS/')
    },
    Ibirama () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Ibirama-RS/')
    },
    Igrejinha () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Igrejinha-RS/')
    },
    Ilopolis () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Ilopolis-RS/')
    },
    Imigrante () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Imigrante-RS/')
    },
    Itati () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Itati-RS/')
    },
    Ivoti () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Ivoti-RS/')
    },
    Imbe () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Imbe-RS/')
    },
    Lagoao () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Lagoao-RS/')
    },
    Lajedo () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Lajedo-RS/')
    },
    LindolfoCollor () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Lindolfo-Collor-RS/')
    },
    LinhaNova () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Linha-Nova-RS/')
    },
    Maquine () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Maquine-RS/')
    },
    MarianaPimentel () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Mariana-Pimentel-RS/')
    },
    MarquesDeSouza () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Marques-de-Souza-RS/')
    },
    MatoLeitao () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Mato-Leitao-RS/')
    },
    MinasDoLeao () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Minas-do-Leao-RS/')
    },
    Montenegro () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Montenegro-RS/')
    },
    MorrinhosDoSul () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Morrinhos-do-Sul-RS/')
    },
    MorroReuter () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Morro-Reuter-RS/')
    },
    Mostardas () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Mostardas-RS/')
    },
    Mucum () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Mucum-RS/')
    },
    NovaBrescia () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Nova-Brescia-RS/')
    },
    NovaHartz () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Nova-Hartz-RS/')
    },
    NovaSantaRita () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Nova-Santa-Rita-RS/')
    },
    NovoHamburgo () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Novo-Hamburgo-RS/')
    },
    Osorio () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Osorio-RS/')
    },
    PalmaresDoSul () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Palmares-do-Sul-RS/')
    },
    PantanoGrande () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Pantano-Grande-RS/')
    },
    PareciNovo () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Pareci-Novo-RS/')
    },
    Parobe () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Parobe-RS/')
    },
    PassoDoSobrado () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Passo-do-Sobrado-RS/')
    },
    Paverema () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Paverema-RS/')
    },
    PoçoDasAntas () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Poço-das-Antas-RS/')
    },
    Portao () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Portao-RS/')
    },
    PortoAlegre () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Porto-Alegre-RS/')
    },
    PousoNovo () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Pouso-Novo-RS/')
    },
    PresidenteLucena () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Presidente-Lucena-RS/')
    },
    Progresso () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Progresso-RS/')
    },
    Putinga () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Putinga-RS/')
    },
    Relvado () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Relvado-RS/')
    },
    RioPardo () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Rio-Pardo-RS/')
    },
    RocaSales () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Roca-Sales-RS/')
    },
    Rolante () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Rolante-RS/')
    },
    Riozinho () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Riozinho-RS/')
    },
    SalvadorDoSul () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Salvador-do-Sul-RS/')
    },
    SantaClaraDoSul () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Santa-Clara-do-Sul-RS/')
    },
    SantaCruzDoSul () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Santa-Cruz-do-Sul-RS/')
    },
    SantaMariaDoHerval () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Santa-Maria-do-Herval-RS/')
    },
    SantoAntonioDaPatrulha () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Santo-Antonio-da-Patrulha-RS/')
    },
    SaoJeronimo () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Sao-Jeronimo-RS/')
    },
    SaoJoseDoHortencio () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Sao-Jose-do-Hortencio-RS/')
    },
    SaoLeopoldo () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Sao-Leopoldo-RS/')
    },
    SaoSebastiaoDoCai () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Sao-Sebastiao-do-Cai-RS/')
    },
    SaoVendelino () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Sao-Vendelino-RS/')
    },
    Sapiranga () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Sapiranga-RS/')
    },
    SapucaiaDoSul () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Sapucaia-do-Sul-RS/')
    },
    Segredo () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Segredo-RS/')
    },
    SentinelaDoSul () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Sentinela-do-Sul-RS/')
    },
    Serio () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Serio-RS/')
    },
    SertaoSantana () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Sertao-Santana-RS/')
    },
    Sinimbu () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Sinimbu-RS/')
    },
    Sobradinho () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Sobradinho-RS/')
    },
    SantanaDoLivramento () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Santana-do-Livramento-RS/')
    },
    Tabai () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Tabai-RS/')
    },
    Tapes () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Tapes-RS/')
    },
    Taquara () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Taquara-RS/')
    },
    Travesseiro () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Travesseiro-RS/')
    },
    Tunas () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Tunas-RS/')
    },
    Taquari () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Taquari-RS/')
    },
    Tavares () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Tavares-RS/')
    },
    TerraDeAreia () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Terra-de-Areia-RS/')
    },
    TresCachoeiras () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Tres-Cachoeiras-RS/')
    },
    TresCoroas () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Tres-Coroas-RS/')
    },
    Tupandi () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Tupandi-RS/')
    },
    Teutonia () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Teutonia-RS/')
    },
    Torres () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Torres-RS/')
    },
    Tramandai () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Tramandai-RS/')
    },
    TresForquilhas () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Tres-Forquilhas-RS/')
    },
    Triunfo () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Triunfo-RS/')
    },
    Uruguaiana () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Uruguaiana-RS/')
    },
    ValeDoSol () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Vale-do-Sol-RS/')
    },
    ValeReal () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Vale-Real-RS/')
    },
    Viamao () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Viamao-RS/')
    },
    ValeVerde () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Vale-Verde-RS/')
    },
    VenancioAires () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Venancio-Aires-RS/')
    },
    VeraCruz () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Vera-Cruz-RS/')
    },
    VespasianoCorreia () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Vespasiano-Correia-RS/')
    },
    XangriLa () {
      this.$router.push('/detetive-particular-no-Rio-Grande-do-Sul/detetive-particular-em-Xangri-La-RS/')
    }
  }
}
</script>
<style scoped>
  .separation-tema{
    position: absolute;
    height: 3px;
    width: 200px;
    bottom: -10px;
    border-radius: 3px;
    background-color: var(--roxo);
  }
  .borda-tema-fina{
    position: absolute;
    height: 2px;
    width: 200px;
    bottom: -1px;
    border-radius: 3px;
    background-color: var(--roxo);
  }
  ol.carousel-indicators li{
    width: 13px !important;
    height: 13px !important;
  }
</style>
