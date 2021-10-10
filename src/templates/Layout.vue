<script setup lang="ts"></script>

<template>
  <div class="layout">
    <header class="header">
      <nav class="nav">
        <ul class="nav-list">
          <li><router-link to="/">Home</router-link></li>
          <li><router-link to="/about">About</router-link></li>
        </ul>
      </nav>
    </header>
    <main class="main">
      <router-view />
    </main>
    <footer class="footer"><p>I am footer</p></footer>
  </div>
</template>

<style>
.layout {
  @apply flex flex-grow flex-col h-screen;
}
.header {
  @apply bg-green-300 flex justify-center h-12;
}
.nav {
  @apply justify-center align-middle h-full;
}
.nav-list {
  @apply flex flex-row flex-nowrap flex-grow h-full bg-red-200;
}
.nav-list li {
  @apply w-auto mx-10;
}

.main {
  @apply bg-green-500 flex flex-grow;
}
.footer {
  @apply h-auto;
  @apply bg-green-700;
}
</style>
