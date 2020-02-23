<template>
  <div class="container">
    <div>
      <logo />
      <h1 class="title">
        nuxt-with-tailwindo
      </h1>
      <h2 class="subtitle">
        My stylish Nuxt.js project
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

<style scoped>
.container {
  @apply font-sans min-h-screen flex justify-center items-center text-center mx-auto;
}

.title {
  @apply font-body block font-light text-indigo-400 tracking-tighter;
  font-size: 100px;
  user-select: all;
  @screen md {
    @apply text-gray-400;
  }
  &:hover {
    @apply text-red-400;
  }
}

.subtitle {
  @apply font-light text-3xl;
  color: #526488;
  &:hover {
    color: theme('colors.blue.500');
  }
}

.links {
  @apply pt-6;
}
</style>
