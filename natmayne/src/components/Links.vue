<template>
  <div class="links">
    <div class="links-container">
      <a :href="'https://github.com/nathanaelmayne'">
        <SVGIcon name="github"/>
      </a>
      <a :href="'https://www.linkedin.com/in/nathanael-mayne-956b83122'">
        <SVGIcon name="linkedIn"/>
      </a>
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
  padding-right: 16px;
}
</style>
