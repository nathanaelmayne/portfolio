<template>
  <div class="hero">
    <h1>
      Hi,
      <br>
      <br>I'm Nathanael Mayne, a
      <b>Web Developer</b> based in
      <i>Hamilton New Zealand</i>.
    </h1>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";

export default {
  components: {}
};
</script>
  
<style scoped lang="scss">
.hero {
  display: flex;
  flex-direction: row;
  padding: 12rem 0 0;
  margin: 0 auto 6rem;
}

b {
  padding: 0.2rem 0.3rem;
  background: $accent;
}

i {
  font-style: normal;
  padding-bottom: 0.2rem;
  border-bottom: $accent solid 0.2rem;
}
</style>
