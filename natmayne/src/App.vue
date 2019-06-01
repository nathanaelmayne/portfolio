<template>
  <div id="app">
    <HeaderBar/>
    <MainPage/>
  </div>
</template>

<style lang="scss">
  @import 'global.scss';
</style>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import MainPage from './components/MainPage.vue';
import HeaderBar from './components/HeaderBar.vue';
import Links from './components/Links.vue';

@Component({
  components: {
    MainPage,
    HeaderBar
  },
})
export default class App extends Vue {}
</script>
