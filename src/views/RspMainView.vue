<template>
  <body>
    <RspHeader></RspHeader>
    <RspMain></RspMain>
    <rsp-footer></rsp-footer>
  </body>
</template>

<script>
import RspHeader from '../components/LottoHeader.vue'
import RspMain from '@/components/rsp/RspMain.vue'
import RspFooter from '../components/LottoFooter.vue'

export default {
  components: {
    RspHeader,
    RspMain,
    RspFooter
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
