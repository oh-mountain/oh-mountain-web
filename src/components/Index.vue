<template>
  <div id="app">
    <!--&lt;!&ndash;PC版&ndash;&gt;-->
    <!--<TopPc v-if="!isMobile()"/>-->
    <!--&lt;!&ndash;SP版&ndash;&gt;-->
    <!--<TopSp v-if="isMobile()"/>-->
    <!--TODO: 一旦PC版を常に出す-->
    <TopPc />
  </div>
</template>

<script>
import detectBrowser from 'detect-browser'
import TopPc from './pc/TopPc'
import TopSp from './sp/TopSp'

const mixinDetictingMobile = {
  methods: {
    isMobile: () => {
      const browser = detectBrowser.detect()
      return (browser.os.indexOf('Android') > -1 || browser.os.indexOf('iOS') > -1)
    }
  }
}

export default {
  components: {TopSp, TopPc},
  mixins: [mixinDetictingMobile],
  name: 'Top',
  created () {
    console.log('loaded Index')
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  h1, h2 {
    font-weight: normal;
  }

  ul {
    list-style-type: none;
    padding: 0;
  }

  li {
    display: inline-block;
    margin: 0 10px;
  }

  a {
    color: #42b983;
  }
</style>
