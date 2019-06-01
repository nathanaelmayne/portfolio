<template>
  <div class="main-page">
    <h1>Hi its the main page</h1>
    <Links/>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";
import Links from "./Links.vue";

@Component({
  components: {
    Links
  }
})
export default class MainPage extends Vue {}
</script>

<style scoped lang="scss">
.main-page {
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>
