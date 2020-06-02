<template>
  <div id="app">
    <Message/>
  </div>
</template>

<script>
import Message from './components/Message';


export default {
  name: 'App',
  components: {
    Message,
  },
  data(){
    
  },
  methods:{
    fetchData(){
    }
  }

}
</script>

<style>
* {
  margin:0;
  padding: 0;
  box-sizing: border-box;
}
</style>
