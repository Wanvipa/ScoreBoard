<template>
  <div class="hello">
<br><br>
  <pa>{{point}}</pa>
    <br><br><br><br><br>

  </div>
</template>

<script>
export default {
  props: ['point'],
  data () {
    return {
      msg: 'Hello World!'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  color: #42b983;
}
pa{
  font-size: 100px;
}
</style>
