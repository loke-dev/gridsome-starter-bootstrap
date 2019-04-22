<template>
  <div class="layout">
    <div id="content-wrapper">
      <header class="header">
        <strong>
          <g-link class="logo-home" to="/">{{ $static.metaData.siteName }}</g-link>
        </strong>
        <nav class="nav">
          <g-link class="nav__link" to="/blog">Blog</g-link>
          <g-link class="nav__link" to="/about">About</g-link>
          <g-link class="nav__link" to="/contact">Contact</g-link>
        </nav>
      </header>
      <slot/>
    </div>
    <Footer/>
  </div>
</template>

<static-query>
query {
  metaData {
    siteName
  }
}
</static-query>

<script>
import Footer from '../components/Footer'
export default {
  components: {
    Footer
  }
}
</script>


<style>
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
  width: 950px;
  margin: 0 auto;
}

.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
  height: 80px;
}

.logo-home {
  font-size: 24px;
}

.nav__link {
  margin-left: 20px;
}

.active--exact {
  font-weight: bold;
}
</style>
