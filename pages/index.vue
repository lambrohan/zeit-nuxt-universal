<template>
  <div class="container">
    <a
      target="_blank"
      class="repo-link"
      href="https://github.com/lambrohan/zeit-nuxt-universal.git"
    >
      <img src="/git.png" />Repository</a
    >
    <div>
      <logo />
      <h1 class="title">
        zeit-nuxt-universal
      </h1>
      <h2 class="subtitle">
        Starting template for Nuxt SSR app on Zeit Now
      </h2>
      <div class="links">
        <a href="https://nuxtjs.org/" target="_blank" class="button--green">
          Documentation
        </a>
        <a
          href="https://github.com/nuxt/nuxt.js"
          target="_blank"
          class="button--grey"
        >
          GitHub
        </a>
      </div>
    </div>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  }
}
</script>

<style lang="scss" scopped>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
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

.repo-link {
  color: inherit;
  text-decoration: none;
  display: flex;
  align-items: center;
  justify-content: center;
  background: #f5f5f5;
  border-radius: 20px;
  box-sizing: border-box;
  padding: 4px 12px;
  transition: 0.3s ease all;
  position: absolute;
  right: 24px;
  top: 24px;

  &:hover {
    box-shadow: 2px 4px 12px rgba(0, 0, 0, 0.096);
  }

  img {
    width: 30px;
    margin-right: 8px;
  }
}
</style>
