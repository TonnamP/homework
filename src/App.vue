<template>
<div id="app">
  <hello></hello>
  <broad-score :score-left="ScoreLeft" :score-right="ScoreRight"></broad-score>
  <score-left :leftadd1="leftadd1" :leftadd2="leftadd2" :leftadd3="leftadd3" :left1="left1" :ScoreLeft="ScoreLeft"></score-left>
  <score-right :rightadd1="rightadd1" :rightadd2="rightadd2" :rightadd3="rightadd3" :right1="right1" :ScoreRight="ScoreRight"></score-right>
</div>
</template>

<script>
import Hello from './components/Hello'
import BroadScore from './components/BroadScore'
import ScoreLeft from './components/ScoreLeft'
import ScoreRight from './components/ScoreRight'
export default {
  data () {
    return {
      ScoreLeft: 0,
      ScoreRight: 0
    }
  },
  components: {
    Hello,
    BroadScore,
    ScoreLeft,
    ScoreRight
  },
  methods: {
    leftadd1: function () {
      this.ScoreLeft = this.ScoreLeft + 1
    },
    leftadd2: function () {
      this.ScoreLeft = this.ScoreLeft + 2
    },
    leftadd3: function () {
      this.ScoreLeft = this.ScoreLeft + 3
    },
    left1: function () {
      this.ScoreLeft--
      if (this.ScoreLeft < 0) {
        this.ScoreLeft = 0
      }
    },
    rightadd1: function () {
      this.ScoreRight = this.ScoreRight + 1
    },
    rightadd2: function () {
      this.ScoreRight = this.ScoreRight + 2
    },
    rightadd3: function () {
      this.ScoreRight = this.ScoreRight + 3
    },
    right1: function () {
      this.ScoreRight--
      if (this.ScoreRight < 0) {
        this.ScoreRight = 0
      }
    }
  }
}
</script>

<style>
html {
  height: 100%;
}

body {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 100%;
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

.btn-disable {
  pointer-events: none;
}
</style>
