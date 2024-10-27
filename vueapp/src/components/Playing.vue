<template>
  <v-main class="queue">
    <h2>Waiting</h2>
    <!-- <Waiting /> -->
  </v-main>
  <v-divider vertical></v-divider>
  <v-main class="queue h-screen">
    <h2>OnDeck</h2>
    <!-- <OnDeck /> -->
  </v-main>
  <v-divider vertical></v-divider>
  <v-main class="courts h-screen">
    <h2>Venue</h2>
    <!-- <Venue /> -->
  </v-main>
</template>

<style>
@import "@/assets/styles/custom.css";
</style>

<script setup lang="ts"></script>
