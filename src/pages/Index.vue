<template>
  <Layout>
    
    <!-- Learn how to use images here: https://gridsome.org/docs/images -->
    <g-image alt="Example image" src="~/favicon.png" width="135" />
    
    <h1 class="mt-5">Hello, world!</h1>

    <div class="my-4">
      <b-button v-b-modal.modal-1>Launch demo modal</b-button>

      <!-- Modal Component -->
      <b-modal id="modal-1" title="BootstrapVue">
        <p class="my-4">Hello from modal!</p>
      </b-modal>
    </div>
   
    <p>
      Lorem ipsum dolor sit amet, consectetur adipisicing elit. Pariatur excepturi labore tempore expedita, et iste tenetur suscipit explicabo! Dolores, aperiam non officia eos quod asperiores
    </p>

    <p class="home-links mt-5">
      <a href="https://gridsome.org/" target="_blank" rel="noopener"><b-button variant="primary">Gridsome</b-button></a>
      <a href="https://github.com/LokeCarlsson/gridsome-starter-bootstrap" target="_blank" rel="noopener"><b-button variant="dark">Starter repo</b-button></a>
    </p>

  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: 'Hello, world!'
  }
}
</script>

<style>
.home-links a {
  margin-right: 1rem;
}
</style>
