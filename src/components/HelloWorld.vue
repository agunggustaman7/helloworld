<template>
  <div class="hello">
    <div class="app-6">
      <input v-model="message" placeholder="isi dulu">
      
      <button v-on:click="tetcConsole">Submit</button>
      <p>{{message}}</p>
    </div> 
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: ""
  },
  data(){
    return {
      message:''
    }
  },
  methods:{
    tetcConsole() {
      alert(this.message)
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
