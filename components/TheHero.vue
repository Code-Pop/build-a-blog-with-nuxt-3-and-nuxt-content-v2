<script setup></script>

<template>
  <section class="hero is-info is-medium is-bold">
    <div class="hero-body">
      <div class="container has-text-centered">
        <h1 class="title is-size-1">
          <slot />
        </h1>
        <slot name="subtitle" />
      </div>
    </div>
  </section>
</template>

<style>
.hero-body {
  background-position: center;
  background-size: cover;
  background-repeat: no-repeat;
  height: 400px;
}
</style>
