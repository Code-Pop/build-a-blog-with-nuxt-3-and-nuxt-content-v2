<script setup>
const currentCount = ref(0)

const incrementCount = () => {
  currentCount.value++
}
</script>

<template>
  <main>
    <TheHero>
      <template v-slot:default>Hard-Coded Blog Post #1</template>

      <template v-slot:subtitle>
        <BlogPostMeta author="@bruno" date="2022-06-01" color="dark" />
      </template>
    </TheHero>
    <div class="container">
      <section class="articles">
        <div class="column is-8 is-offset-2">
          <section class="blog-post-card card article">
            <div class="card-content">
              <div class="content article-body is-size-5">
                <h2 id="second-heading">What is a counter?</h2>
                <p>
                  It allows you to keep track of a number and increment it by
                  clicking on a button.
                </p>
              </div>
              <div class="counter">
                <p class="current-count">
                  Current Count: <strong>{{ currentCount }}</strong>
                </p>
                <button @click="incrementCount">Add 1</button>
              </div>
            </div>
          </section>
        </div>
      </section>
    </div>
  </main>
</template>

<style>
.counter {
  max-width: 500px;
  padding: 15px;
  margin: 0 auto;
  border: 3px solid #ccc;
  text-align: center;
}

.counter .current-count {
  margin-bottom: 10px;
  text-align: center;
  font-size: 1.5rem;
}

.counter button {
  font-size: 1rem;
  padding: 5px;
}
</style>
