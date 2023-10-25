<script setup lang="ts">
import styles from './assets/example.module.css'
import logo from './assets/logo.png'

const logo2 = new URL('./assets/logo.png', import.meta.url).href

console.log(styles)
console.log(logo)
console.log(logo2)
</script>

<template>
  <h1>Hello Vue 3 + Vite</h1>
  <h2>Typescript</h2>
  <div id="post">
    <p>PostCSS</p>
  </div>
  <p :class="styles.example">Hello CSS Modules</p>
  <img alt="Vue logo" :src="logo" />
  <img alt="Vue logo" :src="logo2" />
  <img alt="Vue logo" src="/logo.png" />
</template>

<style>
@import 'assets/main.css';

#post {
  & p {
    color: orange;
  }
}
</style>
