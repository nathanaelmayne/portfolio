<template>
  <div class="hero">
    <h1>
      Hi,
      <br>
      <br>I'm Nathanael Mayne, a 
      <div class="tooltip">
        <span>{{skillList()}}</span>
        Software Engineer
        </div> based in
      <span class="location">Hamilton New Zealand.</span>
    </h1>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";

@Component
export default class Counter extends Vue {
  skills: String[] = [
    "User Interface Design",
    "Prototyping",
    "Front-End",
    "API Development",
    "Agile"
  ];

  skillList(): String {
        return this.skills.join(', ');
  }
}
</script>
  
<style scoped lang="scss">
.hero {
  display: flex;
  flex-direction: row;
  padding: 12rem 0 0;
  margin: 0 auto 6rem;
}

.tooltip {
  padding: 0.2rem 0.3rem;
  background: $accent;
  position: relative;
  display: inline-block;
  cursor: help;
}

.tooltip span {
  visibility: hidden;
  opacity: 0;
  position: absolute;
  z-index: 1;
  bottom: 125%;
  left: 0;
  min-width: 6rem;
  color: rgb(255, 255, 255);
  background: rgb(38, 38, 38);
  font: normal 1.2rem/1.6 "sans", sans-serif;
  padding: 1rem 1.5rem;
  border-radius: 0.2rem;
  -webkit-transition: opacity 0.3s ease-out;
  transition: opacity 0.3s ease-out;
}

.tooltip:hover span {
  visibility: visible;
  opacity: 1;
}

.location {
  font-style: normal;
  padding-bottom: 0.2rem;
  border-bottom: $accent solid 0.2rem;
}
</style>
