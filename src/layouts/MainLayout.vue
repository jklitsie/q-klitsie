<template>
  <q-layout view="lHh Lpr lFf">
    <q-header>
      <q-toolbar>
        <q-toolbar-title> J.K. </q-toolbar-title>
        <div class="row">
          <q-btn :class="{active: routeIsHome}" unelevated to='/' class="q-mr-md">Home</q-btn>
          <q-btn :class="{active: routePortfolio}" unelevated to="/portfolio" class="q-mr-md">Portfolio</q-btn>

        </div>
      </q-toolbar>
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>
    <q-footer class="">

    </q-footer>
  </q-layout>
</template>

<script>
import { defineComponent, ref } from "vue";

export default defineComponent({
  name: "MainLayout",

  components: {

  },

  setup() {
  },
  computed: {
    routePortfolio: function () {
      return this.$route.path === '/portfolio';
    },
    routeIsHome: function () {
      return this.$route.path == '/';
    }
  }
});
</script>
<style lang="scss">
.q-toolbar {
  padding:0px;
}
.q-btn.active {
  text-decoration: underline;
}
</style>
