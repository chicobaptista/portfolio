<template>
  <div>
    <h1>Skills</h1>
    <div class="row">
      <div class="col col-3">
        <img src="../assets/html.jpg">
        <p>HTML</p>
      </div>
      <div class="col col-3">
        <img src="../assets/css.jpg">
        <p>CSS</p>
      </div>
      <div class="col col-3">
        <img src="../assets/java.jpg">
        <p>Javascript</p>
      </div>
      <div class="col col-3">
        <img src="../assets/java.jpg">
        <p>Angular</p>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class Skills extends Vue {
  @Prop() private msg!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>
