<script setup lang="ts"></script>

<template>
  <h1>Hello Vue 3 + Vite</h1>
  <h2>Typescript</h2>
  <div id="post">
    <p>PostCSS</p>
  </div>
</template>

<style>
@import 'assets/main.css';

#post {
  & p {
    color: orange;
  }
}
</style>
