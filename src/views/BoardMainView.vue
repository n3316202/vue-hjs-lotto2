<template>
  <body>
    <BoardHeader></BoardHeader>
    <BoardMain></BoardMain>
    <BoardFooter></BoardFooter>
  </body>
</template>

<script>
import BoardHeader from '../components/LottoHeader.vue'
import BoardMain from '@/components/board/BoardMain.vue'
import BoardFooter from '../components/LottoFooter.vue'

export default {
  components: {
    BoardHeader,
    BoardMain,
    BoardFooter
  }
}
</script>

<style scoped>
body {
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}
</style>
