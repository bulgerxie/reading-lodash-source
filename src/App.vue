<template>
  <div id="app">
    <Sidebar :paths="paths"></Sidebar>
    <div class="content">
      <router-view/>
    </div>
    <a href="https://github.com/bulgerxie/reading-lodash-source" class="github"><icon name="github" scale="2"></icon></a>
  </div>
</template>

<script>
import Sidebar from './components/Sidebar'

export default {
  name: 'App',
  components: {
    Sidebar
  },
  props: {
    paths: Array
  }
}
</script>

<style>
  @import './style/index.scss';
</style>
