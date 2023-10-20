<template>
  <div id="app">
    <!-- <HelloWorld msg="Hello, world."/>
    <PictureComp />
    <TestComp num="10"/> -->

    <ul class="box">
      <li class="item">
        <ClassStyles />
      </li>
      <li class="item">
        <InlineStyles />
      </li>
      <li class="item">
        <CompStyles />
      </li>
      <li class="item">
        <ProgressLine />wefwef
      </li>
    </ul>
    
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
// import PictureComp from './components/Picture.vue'
// import TestComp from './components/Test.vue'

import ClassStyles from './components/ClassStyles.vue'
import InlineStyles from './components/InlineStyles.vue'
import CompStyles from './components/CompStyles.vue'
import ProgressLine from './components/Progress.vue'

export default {
  name: 'App',
  components: {
    // HelloWorld,
    // PictureComp,
    // TestComp,
    ClassStyles,
    InlineStyles,
    CompStyles,
    ProgressLine
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  /* color: red;
  background-color: purple; */
  margin-top: 60px;
  padding: 100px;
  font-size: 2em;
}

.item {
  margin: 30px 0;
  list-style: none;
  border: 1px dotted #000;
}
</style>
