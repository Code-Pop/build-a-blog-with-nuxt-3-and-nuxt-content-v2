<script setup>
useHead({
  title: 'Nuxt 3 Bulma Blog Template',
  link: [
    {
      rel: 'stylesheet',
      href: 'https://maxcdn.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css'
    },
    {
      rel: 'stylesheet',
      href: 'https://cdnjs.cloudflare.com/ajax/libs/overlayscrollbars/1.9.1/css/OverlayScrollbars.min.css'
    },
    {
      rel: 'stylesheet',
      href: 'https://fonts.googleapis.com/css?family=Open+Sans'
    },
    {
      rel: 'stylesheet',
      href: 'https://unpkg.com/bulma@0.9.3/css/bulma.min.css'
    }
  ]
})
</script>

<template>
  <TheNavbar />
  <div>
    <NuxtPage />
  </div>
</template>

<style>
html,
body {
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto,
    Oxygen-Sans, Ubuntu, Cantarell, 'Helvetica Neue', sans-serif;
  font-size: 14px;
  background: #f0f2f4;
}

a {
  color: #3e8ed0;
  transition: color 0.3s ease;
}

a:hover {
  color: #2d628f;
}

.navbar.is-white {
  background: #f0f2f4;
}
.navbar-brand .brand-text {
  font-size: 1.11rem;
  font-weight: bold;
}
.articles {
  margin: 5rem 0;
  margin-top: -200px;
}
.articles .content p {
  line-height: 1.9;
  margin: 15px 0;
}
.author-image {
  position: absolute;
  top: -30px;
  left: 50%;
  width: 60px;
  height: 60px;
  margin-left: -30px;
  border: 3px solid #ccc;
  border-radius: 50%;
}
.media-center {
  display: block;
  margin-bottom: 1rem;
}
.article,
.promo-block {
  margin-top: 6rem;
}
div.column.is-8:first-child {
  padding-top: 0;
  margin-top: 0;
}
.article-title {
  font-size: 2rem;
  font-weight: lighter;
  line-height: 2;
}
.article-subtitle {
  color: #909aa0;
  margin-bottom: 3rem;
}
.article-body {
  line-height: 1.4;
  margin: 0 6rem;
}
.promo-block .container {
  margin: 1rem 5rem;
}
</style>
