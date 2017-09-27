<template>
  <div class="hello" v-bind:title="msg">
    <p v-text="hello"></p>
    <p v-html="hello"></p>
    <h1>{{ msg }}</h1>
    <p>{{num + 1}}</p>
    <p>{{status ? '是' : '否'}}</p>
  </div>
</template>

<script>
export default {
  name: 'hello',
  data () {
    return {
      msg: 'Welcome to demo1',
      hello:'<p>world</p>',
      num:1,
      status:true
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
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
