<template>
  <Layout>
    <parallax speedFactor=0.2 class="parallax-image mb-4">
      <g-image :src="$page.post.image" />
    </parallax>
    <div class="blogPost">
      <h1 v-html="$page.post.title" class="mb-4"/>
      <div class="meta">
        <div class="box author">
          <span class="label">Author</span>
          <span class="author-name" v-text="$page.post.author"/>
        </div>
        <div class="box date">
          <span class="label">Date</span>
          <div v-text="new Date($page.post.date).toLocaleDateString()"/>
        </div>
        <div class="box time">
          <span class="label">Time</span>
          <span>{{ $page.post.timeToRead }} min read</span>
        </div>
      </div>
      <BlogContent class="mt-5" :content="$page.post.content"/>
    </div>
  </Layout>
</template>

<page-query>
query BlogPost ($path: String!) {
  post: blogPost (path: $path) {
    title
    author
    date
    timeToRead
    content
    image
  }
}
</page-query>

<script>
import Parallax from 'vue-parallaxy'
import BlogContent from '@/components/BlogContent'

export default {
  components: {
    Parallax,
    BlogContent,
  },
  metaInfo() {
    return {
      title: this.$page.post.title,
    }
  },
}
</script>

<style lang="scss" scoped>
.meta {
  display: flex;
}

.box {
  display: flex;
  flex-direction: column;
  padding: 0 20px 0 0;
  
  .label {
    font-weight: bold;
  }
}

.Masthead {
  min-height: inherit;
  max-height: 400px;
}
</style>
