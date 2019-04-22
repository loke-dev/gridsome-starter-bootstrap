<template>
  <Layout>
    <h1 class="mb-4">Bootstrap examples</h1>
    
    <b-alert class="mt-4" variant="warning" show>Hello World!</b-alert>

    <div class="my-5">
      <b-card
        title="Card Title"
        img-src="https://picsum.photos/600/300/?image=25"
        img-alt="Image"
        img-top
        tag="article"
        style="max-width: 20rem;"
        class="mb-2"
      >
        <b-card-text>
          Some quick example text to build on the card title and make up the bulk of the card's content.
        </b-card-text>

        <b-button variant="primary" v-b-modal.modal-1>Launch demo modal</b-button>
      </b-card>
      <b-modal id="modal-1" title="BootstrapVue">
        <p class="my-4">Hello from modal!</p>
      </b-modal>
    </div>
  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: 'Examples'
  }
}
</script>

<style>
</style>
