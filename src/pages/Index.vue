<template>
  <div>
    <div class="page-header clear-filter" filter-color="blue">
      <parallax
        class="page-header-image"
        style="background-image: url('img/img1.jpeg')"
      >
      </parallax>
      <div class="container" style="top: 10% !important">
        <div class="content-center brand">
          <img class="n-logo" src="img/logo-tpi-wt.png" alt="" />
          <h1 class="h1-seo">PET Data collector.</h1>
          <h3>
            Aplicacion para recoleccion de datos dobre el reciclaje de PET
          </h3>
          <div class="team">
            <div class="row" style="margin-top: 5em">
              <div class="col-md-6">
                <div class="team-player">
                  <router-link to="/register">
                    <n-button type="primary" size="lg"
                      >Registro</n-button
                    ></router-link
                  >
                </div>
              </div>
              <div class="col-md-6">
                <div class="team-player">
                  <router-link to="/login">
                    <n-button type="primary" size="lg"
                      >Ingreso</n-button
                    ></router-link
                  >
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- <div class="main">
      <div class="section section-images">
        <div class="container">
          <div class="row">
            <div class="col-md-12">
              <div class="hero-images-container">
                <img src="img/hero-image-1.png" alt="" />
              </div>
              <div class="hero-images-container-1">
                <img src="img/hero-image-2.png" alt="" />
              </div>
              <div class="hero-images-container-2">
                <img src="img/hero-image-3.png" alt="" />
              </div>
            </div>
          </div>
        </div>
      </div>
    </div> -->
    <!-- <basic-elements></basic-elements>
    <navigation></navigation>
    <tabs-section></tabs-section>
    <progress-pagination></progress-pagination>
    <notifications></notifications>
    <typography></typography>
    <javascript-components></javascript-components>
    <carousel-section></carousel-section>
    <nucleo-icons-section></nucleo-icons-section>
    <div class="section">
      <div class="container text-center">
        <div class="row justify-content-md-center">
          <div class="col-md-12 col-lg-8">
            <h2 class="title">Completed with examples</h2>
            <h5 class="description">
              The kit comes with three pre-built pages to help you get started
              faster. You can change the text and images and you're good to go.
              More importantly, looking at them will give you a picture of what
              you can built with this powerful Bootstrap 4 ui kit.
            </h5>
          </div>
        </div>
      </div>
    </div>
    <signup-form></signup-form>
    <examples-section></examples-section>
    <download-section></download-section> -->
  </div>
</template>
<script>
import { Parallax, Button } from "@/components";
/*import BasicElements from "./components/BasicElementsSection";
import Navigation from "./components/Navigation";
import TabsSection from "./components/Tabs";
import ProgressPagination from "./components/ProgressPagination";
import Notifications from "./components/Notifications";
import Typography from "./components/Typography";
import JavascriptComponents from "./components/JavascriptComponents";
import CarouselSection from "./components/CarouselSection";
import NucleoIconsSection from "./components/NucleoIconsSection";
import SignupForm from "./components/SignupForm";
import ExamplesSection from "./components/ExamplesSection";
import DownloadSection from "./components/DownloadSection";*/

export default {
  name: "index",
  bodyClass: "index-page",
  components: {
    [Button.name]: Button,
    Parallax,
    /*BasicElements,
    Navigation,
    TabsSection,
    ProgressPagination,
    Notifications,
    Typography,
    JavascriptComponents,
    CarouselSection,
    NucleoIconsSection,
    SignupForm,
    ExamplesSection,
    DownloadSection,*/
  },
};
</script>
<style scoped>
.n-logo {
  max-width: 150px;
}
</style>
