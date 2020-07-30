<template>
  <div id="app">
    <el-container>
    <el-header>
    </el-header>
    <el-container>
      <el-aside width="200px">
        <Sidebar></Sidebar>
      </el-aside>
      <el-container>
        <el-main><router-view/></el-main>
        <el-footer>Footer</el-footer>
      </el-container>
    </el-container>
  </el-container>
  </div>
</template>

<script>
import Sidebar from '../src/components/sub/Sidebar'
export default {
  name: 'App',
  components: {
    Sidebar
  }
}
</script>

<style>
body {
  margin:0px;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.el-header, .el-footer {
    background-color: #B3C0D1;
    color: #333;
    text-align: center;
    line-height: 60px;
  }
  .el-header {
    position: fixed;
    width: 100%;
    top: 0;
    z-index: 99;
  }
  .el-footer {
    position: fixed;
    bottom: 0;
    width: 100%;
  }
  .el-aside {
    background-color: #D3DCE6;
    color: #333;
    text-align: center;
    line-height: 200px;
    min-height: calc(100vh - 60px);
  }
  .el-main {
    background-color: #E9EEF3;
    color: #333;
    text-align: center;
    line-height: 160px;
  }
  body > .el-container {
    margin-bottom: 40px;
  }
</style>
