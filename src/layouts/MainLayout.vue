<template>
  <q-layout view="lHh Lpr lFf">
    <q-header>
      <q-toolbar>
        <q-toolbar-title> J.K. </q-toolbar-title>
        <div class="row">
          <q-btn unelevated to='/' class="q-mr-md">Home</q-btn>
          <q-btn unelevated to="/portfolio" class="q-mr-md">Portfolio</q-btn>

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
});
</script>
