<style>
  body {
    font-family: Helvetica, sans-serif;
  }
</style>

<template>
  <div id="app">
    <h1>{{ msg }}</h1>
    <div style="margin:20px;">
      <editor :model.sync="content"></editor>
    </div>
  </div>
</template>

<script>
  import Editor from './components/summernote.vue';
  export default {
    data () {
      return {     
        msg: 'Hello Vue!',
        content:'Hello World!'
      }
    },
    components:{
      Editor
    }
  }
</script>