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
      <g-image immediate :src="item.node.image" class="mr-3" alt="image" />
      <div class="media-body">
        <h5 class="mt-0">{{item.node.title}}</h5>
        <p class="text-dark">{{item.node.excerpt}}</p>
      </div>
    </div>

    </g-link>
  </Layout>
</template>

<page-query>
query Blog {
	posts: allBlogPost(sortBy: "date") {
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
  }
}

.media-body {
  margin: auto;
}
</style>
