<template>
  <main class="theme-switcher">
    <ThemesColor icon="moon" color="dark" />
    <ThemesColor icon="sun" color="light" />
    <ThemesColor icon="sun" color="nuxt-light" />
    <ThemesColor icon="sun" color="nuxt" />
    <ThemesColor icon="sun" color="nuxt-green" />
  </main>
</template>

<script>
export default {
  data() {
    return {
      colors: [
        'system',
        'light',
        'dark',
        'theme',
        'nuxt',
        'nuxt-green',
        'nuxt-light',
      ],
    }
  },
}
</script>

<style lang="scss">
.theme-switcher {
  height: auto;
  @include flex-col;
  justify-content: center;
}
</style>
