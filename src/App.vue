<template>
  <GlobalLoader>
    <CircleSpinner />
  </GlobalLoader>
  <Notivue v-slot="item">
    <Notifications :item="item" />
  </Notivue>
  <Navbar />
  <RouterView />
</template>
<script setup>
import Navbar from "@/components/Navbar.vue";
import { RouterView } from "vue-router";
import GlobalLoader from "vue-global-loader/GlobalLoader.vue";
import CircleSpinner from "vue-global-loader/CircleSpinner.vue";
import { Notivue, Notifications } from "notivue";
</script>
