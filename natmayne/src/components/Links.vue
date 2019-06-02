<template>
  <div class="links">
    <div class="links-container">
      <SVGIcon name="github"/>
      <SVGIcon name="linkedIn"/>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";
import SVGIcon from "./SVGIcon.vue";

export default {
  components: {
    SVGIcon
  }
};
</script>
  
<style scoped lang="scss">
.links-container > * {
  padding: 8px;
}
</style>
