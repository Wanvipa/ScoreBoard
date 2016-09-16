<template>
<div class="box" border="2">
  <br>
  <h1>Home</h1>
  <score :point="pointHome"></score>
  <button-point :increase-point="increasePointHome" :decrease-point="decreasePointHome"></button-point>
  <br><br><br>
</div>

<div class="box">
  <br>
  <h1>Away</h1>
  <score :point="pointAway"></score>
  <button-point :increase-point="increasePointAway" :decrease-point="decreasePointAway"></button-point>
  <br><br><br>
</div>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/semantic-ui/2.2.4/semantic.min.css" media="screen" title="no title">
<script src="https://cdnjs.cloudflare.com/ajax/libs/semantic-ui/2.2.4/semantic.min.js" charset="utf-8"></script>
</template>

<script>
import Score from './components/Score'
import ButtonPoint from './components/ButtonPoint'

export default {
  data () {
    return {
      pointHome: 0,
      pointAway: 0
    }
  },
  components: {
    Score,
    ButtonPoint
  },
  methods: {
    increasePointHome: function (point) {
      this.pointHome += point
    },
    decreasePointHome: function (point) {
      this.pointHome -= point
    },
    increasePointAway: function (point) {
      this.pointAway += point
    },
    decreasePointAway: function (point) {
      this.pointAway -= point
    }
  }
}
</script>
<style>
html {
  height: 100%;
}

h1 {
  color: #42b983;
  font-size: 700px;
}

.box {
  text-align: center;
  display: inline-block;
  border: 4px solid;
  margin: 1px;
  border-radius: 10px ;
  padding-left: 5px;
  width: 300px;
}

body {
  align-items: center;
  justify-content: center;
  display: flex;
}

#app {
  color: #2c3e50;
  margin-top: -100px;
  max-width: 600px;
  font-family: Source Sans Pro, Helvetica, sans-serif;
  text-align: center;
}

#app a {
  color: #42b983;
  text-decoration: none;
}

.logo {
  width: 100px;
  height: 100px
}
</style>
