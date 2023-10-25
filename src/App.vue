<script setup lang="ts">
import styles from './assets/example.module.css'

console.log(styles)
</script>

<template>
  <h1>Hello Vue 3 + Vite</h1>
  <h2>Typescript</h2>
  <div id="post">
    <p>PostCSS</p>
  </div>
  <p :class="styles.example">Hello CSS Modules</p>
</template>

<style>
@import 'assets/main.css';

#post {
  & p {
    color: orange;
  }
}
</style>
