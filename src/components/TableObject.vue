<template>
  <table>
    <tr v-for="(tableCols, index) in data" :key="tableCols.title">
      <td>{{ tableCols.title }}</td>
    </tr>
    <thead>
      <tr>
        <th v-for="(tableCols, index) in data" :key="index"></th>
      </tr>
    </thead>
  </table>
</template>
<script lang="ts" setup>
import { reactive } from 'vue'

const data = reactive([{ title: 'Hello World' }, { title: 'Lets go' }, { title: 'sdhufsduhf' }])
</script>
<style lang="css" scoped></style>
