<script setup></script>

<template>
  <main>
    <TheHero>
      <template v-slot:default>Hard-Coded Blog Post #1</template>

      <template v-slot:subtitle>
        <BlogPostMeta author="@luisa" date="2022-05-01" color="dark" />
      </template>
    </TheHero>
    <div class="container">
      <section class="articles">
        <div class="column is-8 is-offset-2">
          <section class="blog-post-card card article">
            <div class="card-content">
              <div class="content article-body is-size-5">
                <h1 id="sample-markdown">Sample Markdown</h1>
                <p>This is some basic, sample markdown.</p>
                <h2 id="second-heading">Second Heading</h2>
                <ul>
                  <li>
                    Unordered lists, and:
                    <ol>
                      <li>One</li>
                      <li>Two</li>
                      <li>Three</li>
                    </ol>
                  </li>
                  <li>More</li>
                </ul>
                <blockquote>
                  <p>Blockquote</p>
                </blockquote>
                <p>
                  And <strong>bold</strong>, <em>italics</em>.
                  <a href="https://markdowntohtml.com">A link</a> to somewhere.
                </p>
                <p>And code highlighting:</p>
                <pre><code class="lang-js"><span class="hljs-keyword">var</span> foo = <span class="hljs-string">'bar'</span>;

<span class="hljs-function"><span class="hljs-keyword">function</span> <span class="hljs-title">baz</span><span class="hljs-params">(s)</span> </span>{
   <span class="hljs-keyword">return</span> foo + <span class="hljs-string">':'</span> + s;
}
</code></pre>
                <p>The end ...</p>
              </div>
            </div>
          </section>
        </div>
      </section>
    </div>
  </main>
</template>

<style></style>
