<template>
  <section class="container">
    <div>
      <app-logo/>
      <h1 class="title">
        nuxt-external-redirect
      </h1>
      <h2 class="subtitle">
        Nuxt.js project
      </h2>
      <div class="links">
        <a
          href="/redirect-in"
          target="_blank"
          class="button--grey">redirect(INTERNAL)</a>
        <a
          href="/redirect-in-ego"
          target="_blank"
          class="button--grey">location.href = INTERNAL</a>
        <a
          href="/redirect-in-ego-wait"
          target="_blank"
          class="button--grey">location.href = INTERNAL &amp; return Promise</a>
      </div>
      <div class="links">
        <a
          href="/redirect-ex"
          target="_blank"
          class="button--grey">redirect(EXTERNAL)</a>
        <a
          href="/redirect-ex-ego"
          target="_blank"
          class="button--grey">location.href = EXTERNAL</a>
        <a
          href="/redirect-ex-ego-wait"
          target="_blank"
          class="button--grey">location.href = EXTERNAL &amp; return Promise</a>
      </div>
    </div>
  </section>
</template>

<script>
import AppLogo from '~/components/AppLogo.vue'

export default {
  components: {
    AppLogo
  }
}
</script>

<style>
.container {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
