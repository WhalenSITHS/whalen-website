<template>
  <main class="theme-switcher">
    <ThemesColor icon="moon" color="dark" />
    <ThemesColor icon="sun" color="light" />
    <ThemesColor icon="seedling" color="nuxt" />
    <ThemesColor icon="cloud-moon" color="nuxt-dark" />
    <ThemesColor icon="car-crash" color="outrun" />
    <ThemesColor icon="circle" color="bubblegum" />
    <!--     <ThemesColor icon="user-graduate" color="lucy-2022" />
    <ThemesColor icon="user-graduate" color="knicks" /> -->
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
  width: 60vw;
  margin: 1rem auto;
  justify-content: center;
}
</style>
