<template>
  <div class="page-header clear-filter" filter-color="blue">
    <div
      class="page-header-image"
      style="background-image: url('img/bottles.jpg')"
    ></div>
    <div class="content">
      <div class="container">
        <div class="col-md-5 ml-auto mr-auto">
          <card type="login" plain>
            <div slot="header" class="logo-container">
              <img v-lazy="'img/logo-tpi.png'" alt="" />
            </div>
            <h2>Login</h2>
            <fg-input
              class="no-border input-lg"
              addon-left-icon="now-ui-icons users_circle-08"
              placeholder="Username"
            >
            </fg-input>

            <fg-input
              class="no-border input-lg last-input"
              addon-left-icon="now-ui-icons ui-1_check"
              placeholder="Password"
            >
            </fg-input>

            <template slot="raw-content">
              <div class="card-footer text-center">
                <a
                  href="#/profile"
                  class="btn btn-primary btn-round btn-lg btn-block"
                  >Ingreso</a
                >
              </div>
              <div class="pull-left">
                <h6>
                  <a href="#/register" class="link footer-link">Crear cuenta</a>
                </h6>
              </div>
              <!-- <div class="pull-right">
                <h6>
                  <a href="#pablo" class="link footer-link">Need Help?</a>
                </h6>
              </div> -->
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
  name: "login-page",
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
  width: 100px !important;
  margin-bottom: 25px !important;
}

.last-input {
  margin-bottom: 20px !important;
}
</style>
