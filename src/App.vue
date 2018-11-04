<template>
  <div id="app">
    <TopMenu />
    <Intro />
    <Projects />
    <Skills />
    <Bio />
    <Contact />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import BootstrapVue from 'bootstrap-vue';
Vue.use(BootstrapVue);
import 'bootstrap/dist/css/bootstrap.css';
import 'bootstrap-vue/dist/bootstrap-vue.css';
import HelloWorld from './components/HelloWorld.vue';
import TopMenu from './components/TopMenu.vue';
import Intro from './components/Intro.vue';
import Projects from './components/Projects.vue';
import Skills from './components/Skills.vue';
import Bio from './components/Bio.vue';
import Contact from './components/Contact.vue';

@Component({
  components: {
    HelloWorld,
    TopMenu,
    Intro,
    Projects,
    Skills,
    Bio,
    Contact,
  },
})
export default class App extends Vue {}
</script>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;

  .uppercase {
    text-transform: uppercase;
  }
}
</style>
