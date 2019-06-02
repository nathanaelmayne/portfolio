<template>
  <div class="main-page">
    <Hero/>
    <Links/>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";
import Links from "./Links.vue";
import Hero from "./Hero.vue";

@Component({
  components: {
    Links,
    Hero
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
