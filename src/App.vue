<template>
  <v-app>
    <v-app-bar class="justify-center d-flex" app>
      <v-toolbar-title class="text-center headline text-uppercase">
        <span>Deseja baixar sua bola?</span>
      </v-toolbar-title>
      <v-spacer></v-spacer>
    </v-app-bar>

    <v-content class="flex align-center">
      <BolaList />
    </v-content>
  </v-app>
</template>

<script>
import BolaList from "./components/BolaList";

export default {
  name: "App",
  components: {
    BolaList
  }
};
</script>
