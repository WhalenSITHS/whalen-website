<template>
  <section class="mockup-container section">
    <h1 class="mockup-header">Scrappy Notes</h1>
    <video autoplay muted loop playsinline class="mockup-video">
      <source
        src="https://res.cloudinary.com/dbopxlpuy/video/upload/c_scale,f_auto,w_1200/v1615670019/scrappy notes/scrappy_ynmjah.mov"
      />
    </video>
    <div class="author-banner">
      <h4 class="mockup-created">Created By</h4>
      <div class="authors-list">
        <div class="mockup-author-container">
          <h3 class="mockup-author">Daniel Briskman</h3>
          <h5 class="graduation">SITHS 2022</h5>
        </div>
      </div>

      <p class="mockup-desc">
        This project was designed to show Vue's reactivity and data binding.
        Daniel added a theme switcher because everyone knows having more themes
        is better.
      </p>

      <div class="mockup-links">
        <button
          class="mockup-button-link"
          v-on:click="onClickSite"
          aria-label="Link to the project site"
        >
          Visit
        </button>
        <button
          class="mockup-button-link"
          @click="onClickGit"
          aria-label="Link to the project's Git repo"
        >
          Github
        </button>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  methods: {
    onClickGit() {
      window.open(
        `https://github.com/staten-island-tech/vue-reactivity-project-popplio2`,
        '_blank'
      )
    },
    onClickSite() {
      window.open(`https://scrappynotes.netlify.app/`, '_blank')
    },
  },
}
</script>

<style lang="scss"></style>
