<template>
  <div id="app">
    <Test :msg="msg"></Test>
    <div @click="msg = '1231234'">
      Click here
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import HelloWorld from "./components/HelloWorld.vue";
import { Test } from 'lib';


@Component({
  components: {
    HelloWorld,
    Test
  }
})
export default class App extends Vue {
  msg = 'asdfadsfsadf';
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
