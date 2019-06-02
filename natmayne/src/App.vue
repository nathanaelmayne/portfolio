<template>
  <div id="app">
    <div class="content-container">
      <HeaderBar/>
      <MainPage/>
    </div>
  </div>
</template>

<style lang="scss">
#app {
  display: flex;
  align-items: center;
  justify-content: center;
}

.content-container {
    position: relative;
    max-width: 54rem;
    margin-right: auto;
    margin-left: auto;
    padding-left: 3rem;
    padding-right: 3rem;
}
</style>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import MainPage from "./components/MainPage.vue";
import HeaderBar from "./components/HeaderBar.vue";
import Links from "./components/Links.vue";

@Component({
  components: {
    MainPage,
    HeaderBar
  }
})
export default class App extends Vue {}
</script>
