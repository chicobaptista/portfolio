<template>
  <div>
    <h1>Contact</h1>
    <div class="row">
      <div class="col">
        <p>Do you have any ideas or projects?</p>
        <p>Get in touch and we'll talk about it!</p>
        <p>chico.baptista@gmail.com</p>
        <p><a>Github</a></p>
        <p><a>LinkedIn</a></p>
        <p><a>Steemit</a></p>
      </div>
      <div class="col">
        <form>

        </form>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class Contact extends Vue {
  @Prop() private msg!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>
