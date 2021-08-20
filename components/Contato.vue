<template>
  <div id="contato" class="pt-130">
    <div class="container">
      <h1 class="font-teko position-relative mx-auto col-sm-12 d-flex justify-content-center text-uppercase text-center">
        Contate nossa agência
        <div class="separation-tema" />
      </h1>
      <form autocomplete="off" class="mt-70 px-3 d-flex justify-content-between row" @submit.prevent="submit">
        <div v-show="ShowMsgFixaSuccess" class="py-1 bg-roxo-escuro rounded text-white col-12 mb-4 shadow-sm">
          <p class="d-flex align-items-center mb-0">
            <ion-icon class="fs-20 w-check mr-2" name="checkbox-outline" /> Mensagem enviada com sucesso! Entraremos em contato em breve
          </p>
        </div>
        <div class="form-group w-form-group px-0">
          <input v-model="nome" type="text" :class="{'error-form': $v.nome.$error, 'success-form': SuccessForm}" class="form-control shadow-sm" placeholder="Nome">
          <div v-show="ShowMsgError" v-if="$v.nome.$error" class="error text-left px-2">
            Este campo é obrigatório, mínimo {{ $v.nome.$params.minLength.min }} letras.
          </div>
        </div>
        <div class="form-group w-form-group px-0">
          <input v-model="email" type="text" :class="{'error-form': $v.email.$error, 'success-form': SuccessForm}" class="form-control shadow-sm" placeholder="E-mail">
          <div v-show="ShowMsgError" v-if="$v.email.$error" class="error text-left px-2">
            Digite um E-mail válido
          </div>
        </div>
        <div class="form-group w-form-group px-0">
          <input
            v-model="telefone"
            v-mask="mask"
            type="text"
            :class="{'error-form': $v.telefone.$error, 'success-form': SuccessForm}"
            class="form-control shadow-sm"
            placeholder="Telefone"
            @keypress="VerificaNumero()"
            @keyup.backspace="VerificaNumeroDelete()"
          >
          <div v-show="ShowMsgError" v-if="$v.telefone.$error" class="error text-left px-2">
            Digite um número de telefone válido
          </div>
        </div>
        <div class="form-group w-form-group px-0">
          <input v-model="cidade" type="text" :class="{'error-form': $v.cidade.$error, 'success-form': SuccessForm}" class="form-control shadow-sm" placeholder="Cidade">
          <div v-show="ShowMsgError" v-if="$v.cidade.$error" class="error text-left px-2">
            Em qual cidade você reside?
          </div>
        </div>
        <div class="form-group w-form-group px-0">
          <input v-model="estado" type="text" :class="{'error-form': $v.estado.$error, 'success-form': SuccessForm}" class="form-control shadow-sm" placeholder="Estado">
          <div v-show="ShowMsgError" v-if="$v.estado.$error" class="error text-left px-2">
            Qual o Estado?
          </div>
        </div>
        <div class="form-group w-form-group px-0">
          <select v-model="tipo_servico" :class="{'error-form': $v.tipo_servico.$error, 'success-form': SuccessForm}" class="form-control shadow-sm">
            <option value="" selected disabled>
              Selecione o serviço...
            </option>
            <option value="Investigação conjugal">
              Investigação conjugal
            </option>
            <option value="Investigação empresarial">
              Investigação empresarial
            </option>
            <option value="Investigação política">
              Investigação política
            </option>
            <option value="Localização de pessoas">
              Localização de pessoas
            </option>
          </select>
          <div v-show="ShowMsgError" v-if="$v.tipo_servico.$error" class="error text-left px-2">
            Selecione o tipo de serviço
          </div>
        </div>
        <div class="form-group w-form-group px-0">
          <input v-model="horario_contato" type="text" :class="{'error-form': $v.horario_contato.$error, 'success-form': SuccessForm}" class="form-control shadow-sm" placeholder="Horário para contato">
          <div v-show="ShowMsgError" v-if="$v.horario_contato.$error" class="error text-left px-2">
            Digite um horário para contato
          </div>
        </div>
        <div class="form-group w-form-group px-0">
          <input v-model="data_contato" type="text" :class="{'error-form': $v.data_contato.$error, 'success-form': SuccessForm}" class="form-control shadow-sm" placeholder="Data para contato">
          <div v-show="ShowMsgError" v-if="$v.data_contato.$error" class="error text-left px-2">
            Digite uma data para contato
          </div>
        </div>
        <div class="form-group w-form-group px-0">
          <select v-model="tipo_pessoa" :class="{'error-form': $v.tipo_pessoa.$error, 'success-form': SuccessForm}" class="form-control shadow-sm">
            <option value="" selected disabled>
              Tipo de pessoa...
            </option>
            <option value="Pessoa física">
              Pessoa física
            </option>
            <option value="Pessoa jurírica">
              Pessoa jurírica
            </option>
          </select>
          <div v-show="ShowMsgError" v-if="$v.tipo_pessoa.$error" class="error text-left px-2">
            Selecione o tipo de pessoa
          </div>
        </div>
        <div class="form-group col-12 px-0">
          <textarea v-model="mensagem" :class="{'error-form': $v.mensagem.$error, 'success-form': SuccessForm}" class="form-control shadow-sm" placeholder="Digite sua mensagem" />
          <div v-show="ShowMsgError" v-if="$v.mensagem.$error" class="error text-left px-2">
            Digite uma mensagem
          </div>
        </div>
        <div class="d-flex col-12 px-0 mt-3 justify-content-center">
          <button type="submit" class="btn btn-roxo px-20 btn-lg fs-18 border-radius-0">
            Enviar formulário
          </button>
        </div>
      </form>
      <div class="mt-80 d-flex justify-content-xs-center justify-content-sm-center justify-content-lg-between row mx-auto">
        <div class="col-sm-6 col-lg">
          <h3 class="text-uppercase position-relative d-flex justify-content-center text-center font-teko fw-600">
            Telefones
            <div class="separation-contatos" />
          </h3>
          <h6 class="text-center fs-15 mb-0 mt-20 fw-600">
            Baln. Camboriú
          </h6>
          <div class="d-flex justify-content-center">
            <a href="tel:+" class="text-center">
              <ion-icon class="text-roxo-escuro fs-23" name="call-outline" style="margin-bottom: -4px; margin-left: -7px; margin-right: 2px;" />+55 (00) 0000-0000
            </a>
          </div>
          <h6 class="text-center fs-15 mb-0 mt-10 fw-600">
            Florianópolis
          </h6>
          <div class="d-flex justify-content-center">
            <a href="tel:+" class="text-center">
              <ion-icon class="text-roxo-escuro fs-23" name="call-outline" style="margin-bottom: -4px; margin-left: -7px; margin-right: 2px;" />+55 (00) 0000-0000
            </a>
          </div>
          <h6 class="text-center fs-15 mb-0 mt-10 fw-600">
            Curitiba
          </h6>
          <div class="d-flex justify-content-center">
            <a href="tel:+" class="text-center">
              <ion-icon class="text-roxo-escuro fs-23" name="call-outline" style="margin-bottom: -4px; margin-left: -7px; margin-right: 2px;" />+55 (00) 0000-0000
            </a>
          </div>
          <h6 class="text-center fs-15 mb-0 mt-10 fw-600">
            Caçador
          </h6>
          <div class="d-flex justify-content-center">
            <a href="tel:+" class="text-center">
              <ion-icon class="text-roxo-escuro fs-23" name="call-outline" style="margin-bottom: -4px; margin-left: -7px; margin-right: 2px;" />+55 (00) 0000-0000
            </a>
          </div>
        </div>
        <div class="col-sm-6 mt-xs-40 col-lg mx-lg-40">
          <h3 class="text-uppercase position-relative d-flex justify-content-center text-center font-teko fw-600">
            Redes sociais
            <div class="separation-contatos" />
          </h3>
          <div class="d-flex mt-15 justify-content-center">
            <div>
              <a href="http://" target="_blank" rel="noopener noreferrer" class="fw-500 d-flex align-items-center">
                <ion-icon class="text-roxo-escuro mb-1 mr-2 fs-25" name="logo-facebook" />Facebook
              </a>
              <a href="http://" target="_blank" rel="noopener noreferrer" class="fw-500 mt-10 d-flex align-items-center">
                <ion-icon class="text-roxo-escuro mb-1 mr-2 fs-25" name="logo-twitter" />Twitter
              </a>
              <a href="http://" target="_blank" rel="noopener noreferrer" class="fw-500 mt-10 d-flex align-items-center">
                <ion-icon class="text-roxo-escuro mb-1 mr-2 fs-25" name="logo-instagram" />Instagram
              </a>
              <a href="http://" target="_blank" rel="noopener noreferrer" class="fw-500 mt-10 d-flex align-items-center">
                <ion-icon class="text-roxo-escuro mb-1 mr-2 fs-25" name="logo-youtube" />YouTube
              </a>
              <a href="http://" target="_blank" rel="noopener noreferrer" class="fw-500 mt-10 d-flex align-items-center">
                <ion-icon class="text-roxo-escuro mb-1 mr-2 fs-25" name="logo-pinterest" />Pinterest
              </a>
            </div>
          </div>
        </div>
        <div class="col-md-6 col-lg mt-xs-40 mt-sm-40 mt-lg-0">
          <h3 class="text-uppercase position-relative d-flex justify-content-center text-center font-teko fw-600">
            E-mail
            <div class="separation-contatos" />
          </h3>
          <div class="d-flex mt-15 justify-content-center">
            <a href="mailto:">
              <ion-icon class="text-roxo-escuro fs-25" name="mail-outline" style="margin-bottom: -7px; margin-left: -7px; margin-right: 8px;" />contato@Graziella.com.br
            </a>
          </div>
          <h3 class="text-uppercase position-relative mt-40 d-flex justify-content-center text-center font-teko fw-600">
            Mensagem
            <div class="separation-contatos" />
          </h3>
          <div class="d-flex mt-15 justify-content-center">
            <a class="cursor-pointer" @click.prevent="$root.$emit('ShowModalWhatsapp')">
              <ion-icon class="text-roxo-escuro fs-25" name="logo-whatsapp" style="margin-bottom: -7px; margin-left: -7px; margin-right: 8px;" />+55 (00) 0000-0000
            </a>
          </div>
        </div>
      </div>
    </div>
    <div class="alert-form col-12 pz-0">
      <b-alert
        :show="contadorQueChegaAZero"
        dismissible
        fade
        class="container bg-roxo-escuro border-0 shadow text-white"
        @dismissed="HideAlertMsgSuccess"
        @dismiss-count-down="MetodoParaSumirContador"
      >
        <p class="mb-10 fs-xs-14 d-flex align-items-center">
          <ion-icon class="fs-20 w-check mr-2" name="checkbox-outline" />
          Mensagem enviada com sucesso! Entraremos em contato em breve
        </p>
        <b-progress
          :max="segundosParaSumir -1"
          :value="contadorQueChegaAZero -1"
          height="4px"
        />
      </b-alert>
    </div>
  </div>
</template>
<script>
import Vue from '../node_modules/vue'
import axios from '../node_modules/axios'
import { required, email, minLength } from '../node_modules/vuelidate/lib/validators'
import { VueMaskDirective } from '../node_modules/v-mask'
import Vuelidate from '../node_modules/vuelidate'
Vue.use(Vuelidate)
Vue.directive('mask', VueMaskDirective)
export default {
  data () {
    return {
      nome: '',
      email: '',
      telefone: '',
      cidade: '',
      estado: '',
      tipo_servico: '',
      horario_contato: '',
      data_contato: '',
      tipo_pessoa: '',
      mensagem: '',

      mask: '(##) #####-####',

      SuccessForm: false,
      ShowMsgError: true,

      segundosParaSumir: 9,
      contadorQueChegaAZero: 0,
      showDismissibleAlert: false,
      ShowMsgFixaSuccess: false
    }
  },
  validations: {
    nome: {
      required,
      minLength: minLength(3)
    },
    email: {
      required,
      email
    },
    telefone: {
      required
    },
    cidade: {
      required
    },
    estado: {
      required
    },
    tipo_servico: {
      required
    },
    horario_contato: {
      required
    },
    data_contato: {
      required
    },
    tipo_pessoa: {
      required
    },
    mensagem: {
      required
    }
  },
  methods: {
    submit () {
      this.$v.$touch()
      if (this.$v.$invalid === false) {
        axios.defaults.headers.post['Content-Type'] = 'application/x-www-form-urlencoded'
        axios.post('', JSON.stringify({
          nome: this.nome,
          email: this.email,
          telefone: this.telefone,
          cidade: this.cidade,
          estado: this.estado,
          tipo_servico: this.tipo_servico,
          horario_contato: this.horario_contato,
          data_contato: this.data_contato,
          mensagem: this.mensagem,
          tipo_pessoa: this.tipo_pessoa
        }))
          .then(
            setTimeout(() => {
              this.showAlert()
              this.SuccessForm = true
              this.ShowMsgError = false
              this.nome = ''
              this.email = ''
              this.telefone = ''
              this.cidade = ''
              this.estado = ''
              this.tipo_servico = ''
              this.horario_contato = ''
              this.data_contato = ''
              this.mensagem = ''
              this.tipo_pessoa = ''
            }, 300)
          )
      }
    },
    VerificaNumero () {
      if (window.innerWidth > 992) {
        if (this.telefone.length === 14) {
          this.mask = '(##) # ####-####'
        }
        if (this.telefone.length <= 13) {
          this.mask = '(##) ####-####'
        }
      }
    },
    VerificaNumeroDelete () {
      if (window.innerWidth > 992) {
        if (this.telefone.length <= 15) {
          this.mask = '(##) ####-####'
        }
      }
    },
    MetodoParaSumirContador (contadorQueChegaAZero) {
      this.contadorQueChegaAZero = contadorQueChegaAZero
    },
    showAlert () {
      this.contadorQueChegaAZero = this.segundosParaSumir
    },
    HideAlertMsgSuccess () {
      this.contadorQueChegaAZero = 0
      this.ShowMsgFixaSuccess = true
    }
  }
}
</script>
<style scoped>
  input, textarea{
    border-radius: 0;
    height: 42px;
    padding-left: 20px;
    box-shadow: 0 0.125rem 0.25rem #00000013;
  }
  select{
    border-radius: 0;
    height: 42px;
    padding-left: 17px;
    box-shadow: 0 0.125rem 0.25rem #00000013;
  }
  textarea{
    padding-top: 10px;
    min-height: 130px;
    max-height: 130px;
  }
  input:focus, select:focus, textarea:focus{
    box-shadow: 0 0 0 0.2rem #6c5ce76e !important;
    border-color: #6c5ce76e;
  }
  a{
    color: var(--grafite);
  }
  @media (min-width: 1px) {
    .w-form-group{
      width: 100%;
    }
  }
  @media (min-width: 768px) {
    .w-form-group{
      width: 48.5%;
    }
  }
  @media (min-width: 992px) {
    .w-form-group{
      width: 32.5%;
    }
  }
  .error-form{
    border-color: #f27c87 !important;
    animation-name: AnimateErrorContact;
    -o-animation-name: AnimateErrorContact;
    -moz-animation-name: AnimateErrorContact;
    -webkit-animation-name: AnimateErrorContact;
    animation-duration: 0.5s;
    -o-animation-duration: 0.5s;
    -moz-animation-duration: 0.5s;
    -webkit-animation-duration: 0.5s;
  }
  .error-form:focus{
    box-shadow: 0 0 0 0.2rem rgba(220, 53, 69, 0.25) !important;
  }
  .success-form{
    border: 1px solid #ced4da !important;
    box-shadow: 0 0.125rem 0.25rem #00000013 !important;
  }
  .success-form:focus{
    box-shadow: 0 0 0 0.2rem #6c5ce76e !important;
  }
  @keyframes AnimateErrorContact {
    20%{
      transform: translateX(-5px);
      -o-transform: translateX(-5px);
      -moz-transform: translateX(-5px);
      -webkit-transform: translateX(-5px);
    }
    40%{
      transform: translateX(5px);
      -o-transform: translateX(5px);
      -moz-transform: translateX(5px);
      -webkit-transform: translateX(5px);
    }
    60%{
      transform: translateX(-5px);
      -o-transform: translateX(-5px);
      -moz-transform: translateX(-5px);
      -webkit-transform: translateX(-5px);
    }
    80%{
      transform: translateX(5px);
      -o-transform: translateX(5px);
      -moz-transform: translateX(5px);
      -webkit-transform: translateX(5px);
    }
    100%{
      transform: translateX(0px);
      -o-transform: translateX(0px);
      -moz-transform: translateX(0px);
      -webkit-transform: translateX(0px);
    }
  }
  @-o-keyframes AnimateErrorContact {
    20%{
      transform: translateX(-5px);
      -o-transform: translateX(-5px);
      -moz-transform: translateX(-5px);
      -webkit-transform: translateX(-5px);
    }
    40%{
      transform: translateX(5px);
      -o-transform: translateX(5px);
      -moz-transform: translateX(5px);
      -webkit-transform: translateX(5px);
    }
    60%{
      transform: translateX(-5px);
      -o-transform: translateX(-5px);
      -moz-transform: translateX(-5px);
      -webkit-transform: translateX(-5px);
    }
    80%{
      transform: translateX(5px);
      -o-transform: translateX(5px);
      -moz-transform: translateX(5px);
      -webkit-transform: translateX(5px);
    }
    100%{
      transform: translateX(0px);
      -o-transform: translateX(0px);
      -moz-transform: translateX(0px);
      -webkit-transform: translateX(0px);
    }
  }
  @-moz-keyframes AnimateErrorContact {
    20%{
      transform: translateX(-5px);
      -o-transform: translateX(-5px);
      -moz-transform: translateX(-5px);
      -webkit-transform: translateX(-5px);
    }
    40%{
      transform: translateX(5px);
      -o-transform: translateX(5px);
      -moz-transform: translateX(5px);
      -webkit-transform: translateX(5px);
    }
    60%{
      transform: translateX(-5px);
      -o-transform: translateX(-5px);
      -moz-transform: translateX(-5px);
      -webkit-transform: translateX(-5px);
    }
    80%{
      transform: translateX(5px);
      -o-transform: translateX(5px);
      -moz-transform: translateX(5px);
      -webkit-transform: translateX(5px);
    }
    100%{
      transform: translateX(0px);
      -o-transform: translateX(0px);
      -moz-transform: translateX(0px);
      -webkit-transform: translateX(0px);
    }
  }
  @-webkit-keyframes AnimateErrorContact {
    20%{
      transform: translateX(-5px);
      -o-transform: translateX(-5px);
      -moz-transform: translateX(-5px);
      -webkit-transform: translateX(-5px);
    }
    40%{
      transform: translateX(5px);
      -o-transform: translateX(5px);
      -moz-transform: translateX(5px);
      -webkit-transform: translateX(5px);
    }
    60%{
      transform: translateX(-5px);
      -o-transform: translateX(-5px);
      -moz-transform: translateX(-5px);
      -webkit-transform: translateX(-5px);
    }
    80%{
      transform: translateX(5px);
      -o-transform: translateX(5px);
      -moz-transform: translateX(5px);
      -webkit-transform: translateX(5px);
    }
    100%{
      transform: translateX(0px);
      -o-transform: translateX(0px);
      -moz-transform: translateX(0px);
      -webkit-transform: translateX(0px);
    }
  }
  .error{
    padding: 0 !important;
    margin-top: 5px;
    font-size: 13px;
    font-weight: 500;
    color: #eb5060;
  }
  .w-check{
    min-width: 20px;
    min-height: 20px;
    max-width: 20px;
    max-height: 20px;
  }
  .separation-tema{
    position: absolute;
    height: 3px;
    width: 150px;
    bottom: -10px;
    border-radius: 3px;
    background-color: var(--roxo_escuro);
  }
  .separation-contatos{
    position: absolute;
    height: 3px;
    width: 50px;
    bottom: -4px;
    border-radius: 3px;
    background-color: var(--roxo_escuro);
  }
</style>
