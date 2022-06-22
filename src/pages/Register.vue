<template>
  <div class="page-header clear-filter" filter-color="blue">
    <div
      class="page-header-image"
      style="background-image: url('img/bottles.jpg')"
    ></div>
    <div class="content">
      <div class="container">
        <div class="col-md-5 ml-auto mr-auto">
          <card class="modifiedCard" type="login" plain>
            <div slot="header" class="logo-container">
              <img v-lazy="'img/logo-tpi.png'" alt="" />
            </div>
            <h2 style="width: 140%">Registro</h2>
            <fg-input
              class="no-border input-lg space-inputs"
              addon-left-icon="now-ui-icons users_circle-08"
              placeholder="Nombre compañia"
            >
            </fg-input>

            <fg-input
              class="no-border input-lg space-inputs"
              addon-left-icon="now-ui-icons ui-1_check"
              placeholder="Direccion"
            >
            </fg-input>

            <fg-input
              class="no-border input-lg space-inputs"
              addon-left-icon="now-ui-icons ui-1_check"
              placeholder="Telefono"
            >
            </fg-input>

            <select class="customSelect input-group" id="inputGroupSelect01">
              <option class="customOption" selected>Seleccione Rol</option>
              <option class="customOption" value="1">Centro de acopio</option>
              <option class="customOption" value="2">
                Centro preprocesador
              </option>
              <option class="customOption" value="3">
                Centro transformador
              </option>
            </select>

            <fg-input
              class="no-border input-lg space-inputs"
              addon-left-icon="now-ui-icons ui-1_check"
              placeholder="Nombre responsable"
            >
            </fg-input>

            <fg-input
              class="no-border input-lg space-inputs"
              addon-left-icon="now-ui-icons ui-1_check"
              placeholder="Email"
            >
            </fg-input>

            <fg-input
              class="no-border input-lg space-inputs"
              addon-left-icon="now-ui-icons ui-1_check"
              placeholder="Contraseña"
              type="password"
            >
            </fg-input>

            <template slot="raw-content">
              <div class="card-footer text-center" style="width: 140%">
                <a href="#" class="btn btn-primary btn-round btn-lg btn-block"
                  >Crear cuenta</a
                >
              </div>
            </template>
          </card>
        </div>
      </div>
    </div>
    <!-- <main-footer></main-footer> -->
  </div>
</template>
<script>
import { Card, Button, FormGroupInput } from "@/components";
//import MainFooter from "@/layout/MainFooter";
export default {
  name: "register-page",
  bodyClass: "login-page",
  components: {
    Card,
    //MainFooter,
    [Button.name]: Button,
    [FormGroupInput.name]: FormGroupInput,
  },
};
</script>
<style scoped>
.logo-container {
  width: 80px !important;
  margin-bottom: 25px !important;
  position: relative;
  left: 20%;
}

.space-inputs {
  margin-bottom: 0px !important;
}

.content {
  margin-top: 6% !important;
}

.customSelect {
  background-color: rgba(255, 255, 255, 0.1);
  color: #ffffff;
  padding: 15px 19px;
  border-color: rgba(255, 255, 255, 0);
  border-radius: 30px;
  height: 4em;
  font-weight: 400;
  font-size: 0.8571em;
  margin-bottom: 40px !important;
}

.customOption {
  color: black;
  font-size: 1.2em;
  font-weight: 400;
}

.page-header {
  max-height: 125vh;
}

.modifiedCard {
  margin-left: -40% !important;
}

.input-group {
  width: 140% !important;
}
</style>
