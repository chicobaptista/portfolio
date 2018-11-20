<template>
  <div>
    <h1>Bio</h1>
    <div class="row">
      <div class="col col-6">
        <h4>Education</h4>
        <p>Course name</p>
        <p>Course type</p>
        <p>Course duration</p>
        <p>Institution</p>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class Bio extends Vue {
  @Prop() private msg!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>
