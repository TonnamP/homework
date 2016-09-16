<template>
  <table align="center">
    <tr>
      <td>Away :&nbsp&nbsp
        <button @click="rightadd1">+1</button>
        <button @click="rightadd2">+2</button>
        <button @click="rightadd3">+3</button>
        <button @click="right1">-1</button>
      </td>
    </tr>
  </table>
</template>

<script>
export default {
  props: ['rightadd1', 'rightadd2', 'rightadd3', 'right1', 'ScoreRight']
}
</script>
<style scoped>
h1 {
  color: #FF3300;
}
</style>
