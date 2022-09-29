<template>
  <div class="main-container">
    <Header/>
    <MainBody/>
  </div>
  
</template>

<script>
import Header from './components/Header.vue'
import MainBody from './components/MainBody.vue'

export default {
  name: 'App',
  components: {
    Header,
    MainBody
  }
}
</script>

<style>
  #app {
  max-width: 1600px;
  margin: 0% auto;
}
  .main-container{
    float: left;
    box-sizing: border-box;
    margin: 0%;
    padding: 0%
  }
</style>