<template>
  <div class="layout">
    <div id="content-wrapper">
      <Header/>
      <slot/>
    </div>
    <Footer/>
  </div>
</template>

<script>
import Footer from '../components/Footer'
import Header from '../components/Header'

export default {
  components: {
    Footer,
    Header,
  },
}
</script>


<style lang="scss">
body, html {
  height: 100%;
}

body {
  font-family: -apple-system,system-ui,BlinkMacSystemFont,"Segoe UI",Roboto,"Helvetica Neue",Arial,sans-serif;
  margin:0;
  padding:0;
  line-height: 1.5;
}

#app {
  display: flex;
  flex-direction: column;
  height: 100%;
}

#content-wrapper {
  flex: 1 0 auto;
  max-width: 950px;
  width: 90vw;
  margin: 0 auto;
}
</style>
