<template>
  <div>
    <h1>Hello, my name is Francisco Llamosas</h1>
    <p>I'm a developer that enjoys the whole stack and a blockchain enthusiast</p>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class Intro extends Vue {
  @Prop() private msg!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>
