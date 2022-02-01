<template>
  <section class="mockup-container section">
    <h1 class="mockup-header">FancyTime</h1>
    <video autoplay muted loop playsinline class="mockup-video">
      <source
        src="https://res.cloudinary.com/dbopxlpuy/video/upload/c_scale,f_auto,w_1200/v1615670019/Fancytime/Fancytime_oipzq6.mov"
      />
    </video>
    <div class="author-banner">
      <h4 class="mockup-created">Created By</h4>
      <div class="authors-list">
        <div class="mockup-author-container">
          <h3 class="mockup-author">Queen Karis Ka</h3>
          <h5 class="graduation">SITHS 2024</h5>
        </div>
      </div>

      <p class="mockup-desc">
        Fancytime was developed during Karis's sophomore year of high school.
        The project is designed to teach students about asynchronous JavaScript
        through calling external API's. The project also utilizes Vite. Karis
        choose to use the Animal Crossing API.
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
        `https://github.com/staten-island-tech/api-project-mwah`,
        '_blank'
      )
    },
    onClickSite() {
      window.open(`https://fancy-time.netlify.app/`, '_blank')
    },
  },
}
</script>

<style lang="scss"></style>
