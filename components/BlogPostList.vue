<script setup></script>

<template>
  <div class="container">
    <section class="articles">
      <div class="column is-8 is-offset-2">
        <div class="card article">
          <NuxtLink to="/blog/my-second-blog-post">
            <section class="blog-post-card card article">
              <div class="media">
                <div class="media-content has-text-centered">
                  <h3 class="title article-title has-text-weight-bold">
                    Hard-Coded Blog Post #2
                  </h3>
                  <BlogPostMeta author="@bruno" date="2022-06-01" />
                </div>
              </div>
              <div class="card-content">
                <div class="content article-body is-size-5">
                  Here is the hard-coded description for blog #2.
                </div>
              </div>
            </section>
          </NuxtLink>
        </div>
        <div class="card article">
          <NuxtLink to="/blog/my-first-blog-post">
            <section class="blog-post-card card article">
              <div class="media">
                <div class="media-content has-text-centered">
                  <h3 class="title article-title has-text-weight-bold">
                    Hard-Coded Blog Post #1
                  </h3>
                  <BlogPostMeta author="@luisa" date="2022-05-01" />
                </div>
              </div>
              <div class="card-content">
                <div class="content article-body is-size-5">
                  Here is the hard-coded description for blog #1.
                </div>
              </div>
            </section>
          </NuxtLink>
        </div>
      </div>
    </section>
  </div>
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
