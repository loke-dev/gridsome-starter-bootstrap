<template>
  <Layout>
    <h1 class="my-4 mb-5">Blog</h1>

    <g-link
      :to="item.node.path"
      v-for="item in $page.posts.edges"
      :key="item.node.id"
      class="blog-post"
    >

    <div class="media my-5">
      <g-image :src="item.node.image" class="mr-3" alt="image" />
      <div class="media-body">
        <h5 class="mt-0">{{item.node.title}}</h5>
        {{item.node.excerpt}}
      </div>
    </div>

    </g-link>
  </Layout>
</template>

<page-query>
query Blog {
	posts: allBlogPost {
    edges {
      node {
        id
        path
        title
        excerpt
        image
      }
    }
  }
}
</page-query>

<style lang="scss" scoped>
.media {
  img {
    width: 120px;
    height: 120px;
    object-fit: cover;
    border-radius: 4px;
  }
}

.media-body {
  margin: auto;
}
</style>
