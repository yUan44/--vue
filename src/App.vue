<template>
  <div id="app">
    <button class="small-chiken-root" @click="parentssss()">小鸡跟<i>say</i></button>
    <HelloWorld ref="childddd" />
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld'

export default {
  name: 'App',
  components: {
    HelloWorld
  },
  methods: {
    parentssss () {
      this.$refs.childddd.isHhhh()
    }
  }
}
</script>

<style>
  *{
    margin: 0;
    padding: 0
  }
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
  }
  .small-chiken-root {
    border: 0;
    padding: 4px 10px;
    background: #26f1e7;
    outline: none;
    color: #fff;
    border-radius: 7px;
    cursor: pointer;
    z-index: 999;
    position: absolute;
    top: 20px;
    left: 50%;
    margin-left: -15px;
  }
  .small-chiken-root i {
    font-style: normal;
    font-weight: bold;
    display: inline-block;
    margin-left: 4px;
    color: #2c3e50;
    vertical-align: middle;
    font-size: 16px
  }
</style>
