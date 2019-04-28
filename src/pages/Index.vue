<template>
  <Layout>
    <h1 class="mb-4">
      Hello  and welcome!  
    </h1>

    <g-image class="greet-image" src="../assets/images/hello.svg" />

    <p>
      This is a starter project 
    </p>

    <p class="home-links mt-5">
      <a href="https://github.com/LokeCarlsson/gridsome-starter-bootstrap" target="_blank" rel="noopener"><b-button variant="dark">Github</b-button></a>
    </p>

  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: 'Gridsome starter bootstrap'
  }
}
</script>

<style>
.home-links a {
  margin-right: 1rem;
}

.greet-image {
  display: block;
  margin: auto;
  width: 90%;
  max-width: 500px;
  padding-bottom: 50px;
}
</style>
