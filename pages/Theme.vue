<template>
  <main class="theme-switcher">
    <ThemesColor icon="moon" color="dark" />
    <ThemesColor icon="sun" color="light" />
    <ThemesColor icon="seedling" color="nuxt" />
    <ThemesColor icon="cloud-moon" color="nuxt-dark" />
    <ThemesColor icon="car-crash" color="outrun" />
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
        'outrun',
      ],
    }
  },
}
</script>

<style lang="scss">
.theme-switcher {
  height: auto;
  @include flex-row;
  flex-wrap: wrap;
  width: 70vw;
  margin: 1rem auto;
  align-items: center;
  justify-content: center;
}
@include laptop {
  .theme-switcher {
    width: 80vw;
  }
}
@include tablet {
  .theme-switcher {
    width: 90vw;
    flex-direction: column;
  }
}
</style>
