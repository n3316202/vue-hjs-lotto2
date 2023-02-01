<template>
  <body>
    <lotto-header></lotto-header>
    <lotto-main></lotto-main>
    <lotto-footer></lotto-footer>
  </body>
</template>

<script>
import LottoFooter from '../components/LottoFooter.vue'
import LottoHeader from '../components/LottoHeader.vue'
import LottoMain from '../components/LottoMain.vue'

export default {
  name: 'LottoMainView',
  components: {
    LottoFooter,
    LottoHeader,
    LottoMain
  },
  data() {
    return { lottoSet: new Set() }
  },
  created() {
    console.log(typeof this.lottoSet)
    while (this.lottoSet.size != 6) {
      const lottoNum = Math.ceil(Math.random() * 45 + 1)
      this.lottoSet.add(lottoNum)
    }

    for (let temp of this.lottoSet) {
      console.log(temp)
    }
  },
  methods: {}
}
</script>

<style scoped>
/* body {
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
} */
</style>
