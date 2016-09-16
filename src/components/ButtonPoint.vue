<template>
  <div >
    <button @click="increasePoint(1)"  class="ui yellow button">+1</button>
    <button @click="increasePoint(2)"  class="ui green button">+2</button>
    <button @click="increasePoint(3)"  class="ui blue button">+3</button><br><br>
    <button @click="decreasePoint(1)" class="ui red button">-1</button><br>
  </div>
</template>

<script>
export default {
  props: ['increasePoint', 'decreasePoint'],
  data () {
    return {

    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  color: #42b983;
}

</style>
