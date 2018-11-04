<template>

<b-navbar toggleable="md">
  <b-navbar-toggle target="nav_collapse"></b-navbar-toggle>
  <b-collapse is-nav id="nav_collapse">
    <!-- Right aligned nav items -->
    <b-navbar-nav class="ml-auto">
      <b-nav-item>Home</b-nav-item>
      <b-nav-item>Projects</b-nav-item>
      <b-nav-item>Skills</b-nav-item>
      <b-nav-item>Bio</b-nav-item>
      <b-nav-item>Contact</b-nav-item>
    </b-navbar-nav>
  </b-collapse>
</b-navbar>

</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";

@Component
export default class TopMenu extends Vue {
  @Prop()
  private msg!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
</style>
