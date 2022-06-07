<template>
  <navbar
    position="fixed"
    type="info"
    :transparent="transparent"
    :color-on-scroll="colorOnScroll"
    menu-classes="ml-auto"
  >
    <template>
      <router-link v-popover:popover1 class="navbar-brand" to="/">
        Data collector
      </router-link>
      <!-- <el-popover
        ref="popover1"
        popper-class="popover"
        placement="bottom"
        width="200"
        trigger="hover"
      >
        <div class="popover-body">
          Designed by Invision. Coded by Creative Tim
        </div>
      </el-popover> -->
    </template>
    <template slot="navbar-menu">
      <li class="nav-item">
        <nav-link class="nav-link white" to="/">
          <i class="now-ui-icons business_chart-pie-36"></i> Home
        </nav-link>
      </li>
      <li class="nav-item">
        <nav-link class="nav-link white" to="/login">
          <i class="now-ui-icons business_chart-pie-36"></i> Login
        </nav-link>
      </li>
      <li class="nav-item">
        <nav-link class="nav-link white" to="/">
          <i class="now-ui-icons business_chart-pie-36"></i> Registro
        </nav-link>
      </li>
      <!-- <drop-down
        tag="li"
        title="Components"
        icon="now-ui-icons design_app"
        class="nav-item"
      >
        <nav-link to="/">
          <i class="now-ui-icons business_chart-pie-36"></i> All components
        </nav-link>
        <a
          href="https://demos.creative-tim.com/vue-now-ui-kit/documentation"
          target="_blank"
          class="dropdown-item"
        >
          <i class="now-ui-icons design_bullet-list-67"></i> Documentation
        </a>
      </drop-down> -->
    </template>
  </navbar>
</template>

<script>
import { /*DropDown,*/ Navbar, NavLink } from "@/components";
import { Popover } from "element-ui";
export default {
  name: "main-navbar",
  props: {
    transparent: Boolean,
    colorOnScroll: Number,
  },
  components: {
    //DropDown,
    Navbar,
    NavLink,
    [Popover.name]: Popover,
  },
};
</script>

<style scoped>
.white {
  color: #ffffff;
}
</style>
