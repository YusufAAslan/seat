<template>
  <div id="app">
    <MainMenu />
    <router-view />
  </div>
</template>

<script>
import MainMenu from './components/MainMenu.vue';

export default {
  name: 'App',
  components: {
    MainMenu
  }
};
</script>

<style>
body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
}
</style>
