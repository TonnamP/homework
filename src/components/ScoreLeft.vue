<template>
  <table align="center">
    <tr>
      <td></td>
      <td>Home :
        <button @click="leftadd1">+1</button>
        <button @click="leftadd2">+2</button>
        <button @click="leftadd3">+3</button>
        <button @click="left1">-1</button>
      </td>
    </tr>
  </table>
</template>

<script>
export default {
  props: ['leftadd1', 'leftadd2', 'leftadd3', 'left1', 'ScoreLeft']

}
</script>
<style scoped>
h1 {
  color: #FF3300;
}
</style>
