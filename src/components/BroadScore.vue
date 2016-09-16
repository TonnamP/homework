<template>
<div class="hello">
  <table border="1" align="center" cellspacing="0" width="500">
    <tr>
      <td><h1>Home</h1></td>
      <td><h1>Away</h1></td>
    </tr>
    <tr>
      <td><h2>{{ScoreLeft}}</h2></td>
      <td><h2>{{ScoreRight}}</h2></td>
    </tr>
  </table>
</div>
</template>

<script>
export default {
  props: ['ScoreLeft', 'ScoreRight']
}
</script>
<style scoped>
h1 {
  color: #FF3300;
}
</style>
