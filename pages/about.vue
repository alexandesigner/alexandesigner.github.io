<template>
  <section class="container">
    <h1 class="logo-title">
      <nuxt-link to="/">
        <strong>{</strong><span>alexan</span>designer<strong>}</strong>
      </nuxt-link>
    </h1>
    <h2 class="title">
      This page is loaded from the {{ name }}
    </h2>
    <h3 class="info" v-if="name === 'client'">
      Please refresh the page
    </h3>
    <nuxt-link class="button" to="/">
      Home page
    </nuxt-link>
  </section>
</template>
<script>
export default {
  data ({ req }) {
    return {
      name: req ? 'server' : 'client'
    }
  },
  head () {
    return {
      title: `About Page (${this.name}-side)`
    }
  }
}
</script>

<style scoped>
.info
{
  font-weight: 300;
  color: #0076F8;
  margin: 0;
  margin-top: 10px;
}
.button
{
  margin-top: 50px;
}
</style>
