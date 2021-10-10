<script setup lang="ts">
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup

import Layout from "./templates/Layout.vue";
</script>

<script lang="ts">
const monkey = "Ooga Booga";
const getMonkey = () => {
  return monkey + " 4 6";
};
const thing = "hi dude";
</script>

<template>
  <div class="site-wrapper">
    <Layout />
  </div>
</template>

<style></style>
