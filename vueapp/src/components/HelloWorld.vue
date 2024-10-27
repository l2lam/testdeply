<template>
  <v-layout class="rounded rounded-md h-100">
    <v-app-bar title="Hello">
      <template v-slot:append>
        <v-btn
          icon="mdi-cog"
          v-tooltip="'Club administration'"
        ></v-btn>
        <v-btn
          icon="mdi-play"
          v-tooltip="'Return to playing screen'"
        ></v-btn>
        <v-btn
          icon="mdi-theme-light-dark"
          @click="toggleTheme"
          v-tooltip="isDarkTheme ? 'Switch to light theme' : 'Switch to dark theme'"
        ></v-btn>
      </template>
    </v-app-bar>
  </v-layout>
</template>

<script setup lang="ts">
import { useTheme } from "vuetify";
let isDarkTheme = true;
const theme = useTheme();

function toggleTheme() {
  isDarkTheme = !isDarkTheme;
  theme.global.name.value = isDarkTheme ? "dark" : "light";
}
</script>

