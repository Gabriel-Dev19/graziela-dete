<template>
  <div>
    <Home title-home="Detetive particular em Santa Catarina" :bg-home="true" />
    <section class="pt-100">
      <div class="container">
        <h1 class="font-teko position-relative col-12 px-0 d-flex justify-content-center text-uppercase text-center">
          Contate um detetive particular em Santa Catarina
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
          <div class="separation-tema" />
        </h1>
      </div>
    </section>
    <section class="col-12 mt-50 px-0">
      <div class="container px-xs-0">
        <!-- Cidades A -->
        <div class="position-relative bg-roxo-escuro border border-radius-10 shadow overflow-hidden mt-30 col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-700 mb-1">
              A
            </h5>
          </div>
          <div class="col-lg px-0 mt-4">
            <a class="d-flex col-auto px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Agrolandia">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Agrolândia - SC
            </a>
            <a class="d-flex col-auto px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Agronomica">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Agronômica - SC
            </a>
            <a class="d-flex col-auto px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Apiuna">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Apiúna – SC
            </a>
            <a class="d-flex col-auto px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Araquari">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Araquari – SC
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-auto px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Ascurra">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Ascurra – SC
            </a>
            <a class="d-flex col-auto px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Atalanta">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Atalanta – SC
            </a>
            <a class="d-flex col-auto px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Aurora">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Aurora – SC
            </a>
            <a class="d-flex col-auto px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="AguasMornas">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Águas Mornas – SC
            </a>
            <a class="d-flex col-auto px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="AlfredoWagner">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Alfredo Wagner – SC
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-auto px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Angelina">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Angelina – SC
            </a>
            <a class="d-flex col-auto px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Anitapolis">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Anitápolis – SC
            </a>
            <a class="d-flex col-auto px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="AntonioCarlos">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Antônio Carlos – SC
            </a>
            <a class="d-flex col-auto px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Ararangua">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Araranguá – SC
            </a>
          </div>
        </div>
        <!-- Cidades B -->
        <div class="position-relative bg-roxo-escuro border border-radius-10 shadow mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-700 mb-0">
              B
            </h5>
          </div>
          <div class="col-lg px-0 mt-4">
            <a class="d-flex col-12 px-0 py-0 mt-1 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="BalnearioBarraDoSul">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Balneário Barra do Sul - SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="BalnearioCamboriu">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Balneário Camboriú - SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="BalnearioPicarras">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Balneário Piçarras – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="BarraVelha">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Barra Velha – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="BelaVistaDoToldo">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Bela Vista do Toldo – SC
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="BeneditoNovo">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Benedito Novo – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Blumenau">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Blumenau – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Bombinhas">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Bombinhas – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Botuvera">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Botuverá – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="BracoDoTrombudo">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Braço do Trombudo – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Brusque">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Brusque – SC
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="BalnearioArroioDoSilva">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Balneário Arroio do Silva – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="BalnearioGaivota">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Balneário Gaivota – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="BalnearioRincao">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Balneário Rincão – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Biguacu">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Biguaçu – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="BracoDoNorte">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Braço do Norte – SC
            </a>
          </div>
        </div>
        <!-- Cidades C -->
        <div class="position-relative bg-roxo-escuro border border-radius-10 shadow mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-700 mb-0">
              C
            </h5>
          </div>
          <div class="col-lg px-0 mt-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Camboriu">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Camboriú – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Cacador">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Caçador – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="CamposNovos">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Campos Novos – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Chapeco">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Chapecó – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Concordia">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Concórdia – SC
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="CampoAlegre">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Campo Alegre – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Canoinhas">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Canoinhas – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="ChapadaoDoLageado">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Chapadão do Lageado – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Corupa">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Corupá – SC
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Canelinha">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Canelinha – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="CapivariDeBaixo">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Capivari de Baixo – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="CocalDoSul">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Cocal do Sul – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Criciuma">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Criciúma – SC
            </a>
          </div>
        </div>
        <!-- Cidades D -->
        <div class="position-relative bg-roxo-escuro border border-radius-10 shadow mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-700 mb-0">
              D
            </h5>
          </div>
          <div class="col-lg mt-4 px-0">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="DonaEmma">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Dona Emma – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="DoutorPedrinho">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Doutor Pedrinho – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="DionisioCerqueira">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Dionísio Cerqueira – SC
            </a>
          </div>
        </div>
        <!-- Cidades E -->
        <div class="position-relative bg-roxo-escuro border border-radius-10 shadow mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-700 mb-0">
              E
            </h5>
          </div>
          <a class="d-flex col-12 mt-4 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Ermo">
            <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Ermo – SC
          </a>
        </div>
        <!-- Cidades F -->
        <div class="position-relative bg-roxo-escuro border border-radius-10 shadow mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-700 mb-0">
              F
            </h5>
          </div>
          <a class="d-flex col-12 mt-4 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Florianopolis">
            <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Florianópolis – SC
          </a>
          <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Forquilhinha">
            <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Forquilhinha – SC
          </a>
          <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Fraiburgo">
            <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Fraiburgo – SC
          </a>
        </div>
        <!-- Cidades G -->
        <div class="position-relative bg-roxo-escuro border border-radius-10 shadow mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-700 mb-0">
              G
            </h5>
          </div>
          <div class="col-lg px-0 mt-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Garuva">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Garuva – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Gaspar">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Gaspar – SC
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Guabiruba">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Guabiruba – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Guanamirim">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Guanamirim – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="GovernadorCelsoRamos">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Gov. Celso Ramos – SC
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="GraoPara">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Grão Pará – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Gravatal">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Gravatal – SC
            </a>
          </div>
        </div>
        <!-- Cidades I -->
        <div class="position-relative bg-roxo-escuro border border-radius-10 shadow mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-700 mb-0">
              I
            </h5>
          </div>
          <div class="col-lg px-0 mt-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Ibirama">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Ibirama – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Ilhota">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Ilhota – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Imbuia">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Imbuia – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Indaial">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Indaial – SC
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Irineopolis">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Irineópolis – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Itaiopolis">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Itaiópolis – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Itajai">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Itajaí – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Itapema">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Itapema – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Itapoa">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Itapoá – SC
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Ituporanga">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Ituporanga – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Icara">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Içara – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Imarui">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Imaruí – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Imbituba">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Imbituba – SC
            </a>
          </div>
        </div>
        <!-- Cidades J -->
        <div class="position-relative bg-roxo-escuro border border-radius-10 shadow mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-700 mb-0">
              J
            </h5>
          </div>
          <div class="col-lg px-0 mt-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Joinville">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Joinville – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="JaraguaDoSul">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Jaraguá do Sul – SC
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="JoseBoiteux">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> José Boiteux – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="JacintoMachado">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Jacinto Machado – SC
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Jaguaruna">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Jaguaruna – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Joacaba">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Joaçaba – SC
            </a>
          </div>
        </div>
        <!-- Cidades L -->
        <div class="position-relative bg-roxo-escuro border border-radius-10 shadow mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-700 mb-0">
              L
            </h5>
          </div>
          <div class="col-lg px-0 mt-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Laurentino">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Laurentino – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Lages">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Lages – SC
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Laguna">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Laguna – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="LauroMuller">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Lauro Muller – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="LeobertoLeal">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Leoberto Leal – SC
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Lontras">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Lontras – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="LuisAlves">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Luís Alves – SC
            </a>
          </div>
        </div>
        <!-- Cidades M -->
        <div class="position-relative bg-roxo-escuro border border-radius-10 shadow mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-700 mb-0">
              M
            </h5>
          </div>
          <div class="col-lg px-0 mt-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Mafra">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Mafra – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="MajorVieira">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Major Vieira – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Massaranduba">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Massaranduba – SC
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="MajorGercino">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Major Gercino – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Maracaja">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Maracajá – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="MorroDaFumaca">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Morro da Fumaça – SC
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="MirimDoce">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Mirim Doce – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="MonteCastelo">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Monte Castelo – SC
            </a>
            <a class="d-flex col-12 px-0 mt-1 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="MorroGrande">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Morro Grande – SC
            </a>
          </div>
        </div>
        <!-- Cidades N -->
        <div class="position-relative bg-roxo-escuro border border-radius-10 shadow mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-700 mb-0">
              N
            </h5>
          </div>
          <a class="d-flex col-12 mt-4 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Navegantes">
            <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Navegantes – SC
          </a>
          <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="NovaTrento">
            <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Nova Trento – SC
          </a>
        </div>
        <!-- Cidades O -->
        <div class="position-relative bg-roxo-escuro border border-radius-10 shadow mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-700 mb-0">
              O
            </h5>
          </div>
          <a class="d-flex col-12 mt-4 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Orleans">
            <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Orleans – SC
          </a>
        </div>
        <!-- Cidades P -->
        <div class="position-relative bg-roxo-escuro border border-radius-10 shadow mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-700 mb-0">
              P
            </h5>
          </div>
          <div class="col-lg px-0 mt-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Papanduva">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Papanduva – SC
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Penha">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Penha – SC
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Petrolandia">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Petrolândia – SC
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Picarras">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Piçarras – SC
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Pomerode">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Pomerode – SC
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="PortoBelo">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Porto Belo – SC
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="PousoRedondo">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Pouso Redondo – SC
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="PresidenteGetulio">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Presidente Getúlio – SC
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="PresidenteNereu">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Presidente Nereu – SC
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Palhoca">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Palhoça – SC
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="PassoDeTorres">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Passo de Torres – SC
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="PauloLopes">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Paulo Lopes – SC
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="PedrasGrandes">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Pedras Grandes – SC
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="PescariaBrava">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Pescaria Brava – SC
            </a>
          </div>
        </div>
        <!-- Cidades R -->
        <div class="position-relative bg-roxo-escuro border border-radius-10 shadow mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-700 mb-0">
              R
            </h5>
          </div>
          <div class="col-lg px-0 mt-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="RioDoCampo">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Rio do Campo – SC
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="RioDoOeste">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Rio do Oeste – SC
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="RioFortuna">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Rio Fortuna – SC
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="RioNegrinho">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Rio Negrinho – SC
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Rodeio">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Rodeio – SC
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="RanchoQueimado">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Rancho Queimado – SC
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="RioDoSul">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Rio do Sul – SC
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="RioDosCedros">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Rio dos Cedros – SC
            </a>
          </div>
        </div>
        <!-- Cidades S -->
        <div class="position-relative bg-roxo-escuro border border-radius-10 shadow mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-700 mb-0">
              S
            </h5>
          </div>
          <div class="col-lg px-0 mt-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Salete">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Salete – SC
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="SantaTerezinha">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Santa Terezinha - SC
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="SaoBentoDoSul">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> São Bento do Sul - SC
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="SaoFranciscoDoSul">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> São Francisco do Sul - SC
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="SaoJoaquim">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> São Joaquim - SC
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="SaoJoaoDoItaperiu">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> São João do Itaperiú – SC
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Shroeder">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Shroeder – SC
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Sangao">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Sangão – SC
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="SantaRosaDeLima">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Santa Rosa de Lima – SC
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="SantoAmaroDaImperatriz">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Santo Amaro da Imperatriz – SC
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="SaoBonifacio">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> São Bonifácio – SC
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="SaoJoaoBatista">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> São Jõao Batista – SC
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="SaoJoaoDoSul">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> São Jõao do Sul – SC
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="SaoJose">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> São José – SC
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="SaoLudgero">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> São Ludgero – SC
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="SaoMartinho">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> São Martinho – SC
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="SaoPedroDeAlcantara">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> São Pedro de Alcântara – SC
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Sideropolis">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Siderópolis – SC
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Sombrio">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Sombrio – SC
            </a>
          </div>
        </div>
        <!-- Cidades T -->
        <div class="position-relative bg-roxo-escuro border border-radius-10 shadow mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-700 mb-0">
              T
            </h5>
          </div>
          <div class="col-lg px-0 mt-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Taio">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Taió – SC
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Timbo">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Timbó – SC
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="TrombudoCentral">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Trombudo Central – SC
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Treviso">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Treviso – SC
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="TrezeDeMaio">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Treze de Maio – SC
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Tubarao">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Tubarão – SC
            </a>
          </div>
          <div class="col-lg px-0 mt-lg-4">
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Tijucas">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Tijucas – SC
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="TimbeDoSul">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Timbé do Sul – SC
            </a>
            <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Turvo">
              <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Turvo – SC
            </a>
          </div>
        </div>
        <!-- Cidades U -->
        <div class="position-relative bg-roxo-escuro border border-radius-10 shadow mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-700 mb-0">
              U
            </h5>
          </div>
          <a class="d-flex col-12 mt-4 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Urussanga">
            <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Urussanga – SC
          </a>
          <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Urubici">
            <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Urubici – SC
          </a>
        </div>
        <!-- Cidades V -->
        <div class="position-relative bg-roxo-escuro border border-radius-10 shadow mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-700 mb-0">
              V
            </h5>
          </div>
          <a class="d-flex col-12 px-0 mt-4 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="VidalRamos">
            <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Vidal Ramos – SC
          </a>
          <a class="d-flex col-12 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="VitorMeireles">
            <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Vitor Meireles – SC
          </a>
        </div>
        <!-- Cidades W -->
        <div class="position-relative bg-roxo-escuro border border-radius-10 shadow mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-700 mb-0">
              W
            </h5>
          </div>
          <a class="d-flex col-12 mt-4 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Witmarsum">
            <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Witmarsum – SC
          </a>
        </div>
        <!-- Cidades X -->
        <div class="position-relative bg-roxo-escuro border border-radius-10 shadow mt-30 overflow-hidden col-12 d-flex row mx-auto pr-0 pt-1 pb-30 pl-65">
          <div class="d-flex div-bolinha-letra-cidade justify-content-center align-items-center">
            <h5 class="fw-700 mb-0">
              X
            </h5>
          </div>
          <a class="d-flex col-12 mt-4 px-0 py-0 text-preto-cidades fs-sm-18 fw-600 btn align-items-center" @click.prevent="Xanxere">
            <ion-icon class="fs-20 text-vermelho mr-2" name="navigate-circle-outline" /> Xanxerê – SC
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
    title: 'Detetive particular em Santa Catarina - Agência de detetives Graziella Bastos'
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
    Agrolandia () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Agrolandia-SC/')
    },
    Agronomica () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Agronomica-SC/')
    },
    Apiuna () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Apiuna-SC/')
    },
    Araquari () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Araquari-SC/')
    },
    Ascurra () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Ascurra-SC/')
    },
    Atalanta () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Atalanta-SC/')
    },
    Aurora () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Aurora-SC/')
    },
    AguasMornas () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Aguas-Mornas-SC/')
    },
    AlfredoWagner () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Alfredo-Wagner-SC/')
    },
    Angelina () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Angelina-SC/')
    },
    Anitapolis () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Anitapolis-SC/')
    },
    AntonioCarlos () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Antonio-Carlos-SC/')
    },
    Ararangua () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Ararangua-SC/')
    },
    BalnearioBarraDoSul () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Balneario-Barra-do-Sul-SC/')
    },
    BalnearioCamboriu () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Balneario-Camboriu-SC/')
    },
    BalnearioPicarras () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Balneario-Picarras-SC/')
    },
    BarraVelha () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Barra-Velha-SC/')
    },
    BelaVistaDoToldo () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Bela-Vista-do-Toldo-SC/')
    },
    BeneditoNovo () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Benedito-Novo-SC/')
    },
    Blumenau () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Blumenau-SC/')
    },
    Bombinhas () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Bombinhas-SC/')
    },
    Botuvera () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Botuvera-SC/')
    },
    BracoDoTrombudo () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Braco-do-Trombudo-SC/')
    },
    Brusque () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Brusque-SC/')
    },
    BalnearioArroioDoSilva () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Balneario-Arroio-do-Silva-SC/')
    },
    BalnearioGaivota () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Balneario-Gaivota-SC/')
    },
    BalnearioRincao () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Balneario-Rincao-SC/')
    },
    Biguacu () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Biguacu-SC/')
    },
    BracoDoNorte () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Braco-do-Norte-SC/')
    },
    Camboriu () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Camboriu-SC/')
    },
    Cacador () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Cacador-SC/')
    },
    CamposNovos () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Campos-Novos-SC/')
    },
    Chapeco () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Chapeco-SC/')
    },
    Concordia () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Concordia-SC/')
    },
    CampoAlegre () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Campo-Alegre-SC/')
    },
    Canoinhas () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Canoinhas-SC/')
    },
    ChapadaoDoLageado () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Chapadao-do-Lageado-SC/')
    },
    Corupa () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Corupa-SC/')
    },
    Canelinha () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Canelinha-SC/')
    },
    CapivariDeBaixo () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Capivari-de-Baixo-SC/')
    },
    CocalDoSul () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Cocal-do-Sul-SC/')
    },
    Criciuma () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Criciuma-SC/')
    },
    DonaEmma () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Dona-Emma-SC/')
    },
    DoutorPedrinho () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Doutor-Pedrinho-SC/')
    },
    DionisioCerqueira () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Dionisio-Cerqueira-SC/')
    },
    Ermo () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Ermo-SC/')
    },
    Florianopolis () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Florianopolis-SC/')
    },
    Forquilhinha () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Forquilhinha-SC/')
    },
    Fraiburgo () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Fraiburgo-SC/')
    },
    Garuva () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Garuva-SC/')
    },
    Gaspar () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Gaspar-SC/')
    },
    Guabiruba () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Guabiruba-SC/')
    },
    Guanamirim () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Guanamirim-SC/')
    },
    GovernadorCelsoRamos () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Governador-Celso-Ramos-SC/')
    },
    GraoPara () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Grao-Para-SC/')
    },
    Gravatal () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Gravatal-SC/')
    },
    Ibirama () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Ibirama-SC/')
    },
    Ilhota () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Ilhota-SC/')
    },
    Imbuia () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Imbuia-SC/')
    },
    Indaial () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Indaial-SC/')
    },
    Irineopolis () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Irineopolis-SC/')
    },
    Itaiopolis () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Itaiopolis-SC/')
    },
    Itajai () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Itajai-SC/')
    },
    Itapema () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Itapema-SC/')
    },
    Itapoa () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Itapoa-SC/')
    },
    Ituporanga () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Ituporanga-SC/')
    },
    Icara () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Icara-SC/')
    },
    Imarui () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Imarui-SC/')
    },
    Imbituba () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Imbituba-SC/')
    },
    Joinville () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Joinville-SC/')
    },
    JaraguaDoSul () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Jaragua-do-Sul-SC/')
    },
    JoseBoiteux () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Jose-Boiteux-SC/')
    },
    JacintoMachado () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Jacinto-Machado-SC/')
    },
    Jaguaruna () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Jaguaruna-SC/')
    },
    Joacaba () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Joacaba-SC/')
    },
    Laurentino () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Laurentino-SC/')
    },
    Lages () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Lages-SC/')
    },
    Laguna () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Laguna-SC/')
    },
    LauroMuller () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Lauro-Muller-SC/')
    },
    LeobertoLeal () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Leoberto-Leal-SC/')
    },
    Lontras () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Lontras-SC/')
    },
    LuisAlves () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Luis-Alves-SC/')
    },
    Mafra () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Mafra-SC/')
    },
    MajorVieira () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Major-Vieira-SC/')
    },
    Massaranduba () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Massaranduba-SC/')
    },
    MajorGercino () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Major-Gercino-SC/')
    },
    Maracaja () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Maracaja-SC/')
    },
    MorroDaFumaca () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Morro-da-Fumaca-SC/')
    },
    MirimDoce () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Mirim-Doce-SC/')
    },
    MonteCastelo () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Monte-Castelo-SC/')
    },
    MorroGrande () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Morro-Grande-SC/')
    },
    Navegantes () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Navegantes-SC/')
    },
    NovaTrento () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Nova-Trento-SC/')
    },
    Orleans () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Orleans-SC/')
    },
    Papanduva () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Papanduva-SC/')
    },
    Penha () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Penha-SC/')
    },
    Petrolandia () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Petrolandia-SC/')
    },
    Picarras () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Picarras-SC/')
    },
    Pomerode () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Pomerode-SC/')
    },
    PortoBelo () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Porto-Belo-SC/')
    },
    PousoRedondo () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Pouso-Redondo-SC/')
    },
    PresidenteGetulio () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Presidente-Getulio-SC/')
    },
    PresidenteNereu () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Presidente-Nereu-SC/')
    },
    Palhoca () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Palhoca-SC/')
    },
    PassoDeTorres () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Passo-de-Torres-SC/')
    },
    PauloLopes () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Paulo-Lopes-SC/')
    },
    PedrasGrandes () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Pedras-Grandes-SC/')
    },
    PescariaBrava () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Pescaria-Brava-SC/')
    },
    RioDoCampo () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Rio-do-Campo-SC/')
    },
    RioDoOeste () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Rio-do-Oeste-SC/')
    },
    RioFortuna () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Rio-Fortuna-SC/')
    },
    RioNegrinho () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Rio-Negrinho-SC/')
    },
    Rodeio () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Rodeio-SC/')
    },
    RanchoQueimado () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Rancho-Queimado-SC/')
    },
    RioDoSul () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Rio-do-Sul-SC/')
    },
    RioDosCedros () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Rio-dos-Cedros-SC/')
    },
    Salete () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Salete-SC/')
    },
    SantaTerezinha () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Santa-Terezinha-SC/')
    },
    SaoBentoDoSul () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Sao-Bento-do-Sul-SC/')
    },
    SaoFranciscoDoSul () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Sao-Francisco-do-Sul-SC/')
    },
    SaoJoaquim () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Sao-Joaquim-SC/')
    },
    SaoJoaoDoItaperiu () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Sao-Joao-do-Itaperiu-SC/')
    },
    Shroeder () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Shroeder-SC/')
    },
    Sangao () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Sangao-SC/')
    },
    SantaRosaDeLima () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Santa-Rosa-de-Lima-SC/')
    },
    SantoAmaroDaImperatriz () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Santo-Amaro-da-Imperatriz-SC/')
    },
    SaoBonifacio () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Sao-Bonifacio-SC/')
    },
    SaoJoaoBatista () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Sao-Joao-Batista-SC/')
    },
    SaoJoaoDoSul () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Sao-Joao-do-Sul-SC/')
    },
    SaoJose () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Sao-Jose-SC/')
    },
    SaoLudgero () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Sao-Ludgero-SC/')
    },
    SaoMartinho () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Sao-Martinho-SC/')
    },
    SaoPedroDeAlcantara () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Sao-Pedro-de-Alcantara-SC/')
    },
    Sideropolis () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Sideropolis-SC/')
    },
    Sombrio () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Sombrio-SC/')
    },
    Taio () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Taio-SC/')
    },
    Timbo () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Timbo-SC/')
    },
    TrombudoCentral () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Trombudo-Central-SC/')
    },
    Treviso () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Treviso-SC/')
    },
    TrezeDeMaio () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Treze-de-Maio-SC/')
    },
    Tubarao () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Tubarao-SC/')
    },
    Tijucas () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Tijucas-SC/')
    },
    TimbeDoSul () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Timbe-do-Sul-SC/')
    },
    Turvo () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Turvo-SC/')
    },
    Urussanga () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Urussanga-SC/')
    },
    Urubici () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Urubici-SC/')
    },
    VidalRamos () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Vidal-Ramos-SC/')
    },
    VitorMeireles () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Vitor-Meireles-SC/')
    },
    Witmarsum () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Witmarsum-SC/')
    },
    Xanxere () {
      this.$router.push('/detetive-particular-em-Santa-Catarina/detetive-particular-em-Xanxere-SC/')
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
    background-color: var(--roxo_escuro);
  }
  .borda-tema-fina{
    position: absolute;
    height: 2px;
    width: 200px;
    bottom: -1px;
    border-radius: 3px;
    background-color: var(--roxo_escuro);
  }
  ol.carousel-indicators li{
    width: 13px !important;
    height: 13px !important;
  }
</style>
