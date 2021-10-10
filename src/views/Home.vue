<script setup lang="ts">
import { ref } from "vue";
const staticVariable = "I am staticus";
const count = ref(0);

function changeCount(isIncrement: boolean) {
  isIncrement ? count.value++ : count.value--;
}
</script>

<template>
  <div class="home">
    <p>I am home</p>
    <p>staticVariable: {{ staticVariable }}</p>
    <p>The count is: {{ count }}</p>
    <button @click="changeCount(true)">Increment</button>
    <button @click="changeCount(false)">Decrement</button>
  </div>
</template>
<style>
.home {
  @apply flex flex-col justify-center items-center flex-grow;
}
.title {
}
</style>
