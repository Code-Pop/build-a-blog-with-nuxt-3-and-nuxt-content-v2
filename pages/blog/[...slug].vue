<script setup>
const { path } = useRoute()

const { data: blogPost } = await useAsyncData(`content-${path}`, () => {
  return queryContent().where({ _path: path }).findOne()
})
</script>

<template>
  <main>
    <TheHero>
      <template v-slot:default>{{ blogPost.title }}</template>

      <template v-slot:subtitle>
        <BlogPostMeta
          :author="blogPost.author"
          :date="blogPost.dates.published"
          color="dark"
        />
      </template>
    </TheHero>
    <div class="container">
      <section class="articles">
        <div class="column is-8 is-offset-2">
          <section class="blog-post-card card article">
            <div class="card-content">
              <div class="content article-body is-size-5">
                <ContentDoc />
              </div>
            </div>
          </section>
        </div>
      </section>
    </div>
  </main>
</template>

<style>
.blog-post-card {
  padding-top: 2.5rem;
  padding-bottom: 3rem;
}

.blog-post-card .card-content {
  padding: 1rem;
}

.blog-post-card .title {
  margin-bottom: 1rem;
}
</style>
