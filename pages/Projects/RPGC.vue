<template>
  <section class="mockup-container section">
    <h1 class="mockup-header">RPG Character Designer</h1>
    <video autoplay muted loop playsinline class="mockup-video">
      <source
        src="https://res.cloudinary.com/dbopxlpuy/video/upload/c_scale,f_auto,w_1200/v1615670019/RPG%20Character/AlstonRPG_bnyc1q.mov"
      />
    </video>
    <div class="author-banner">
      <h4 class="mockup-created">Created By</h4>
      <div class="authors-list">
        <div class="mockup-author-container">
          <h3 class="mockup-author">Alston Chan</h3>
          <h5 class="graduation">SITHS 2022</h5>
        </div>
      </div>

      <p class="mockup-desc">
        This project was designed to illustrate Vue's reactivity and data
        binding. The project also allows the user to download an image of the
        character they designed.
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
        `https://github.com/staten-island-tech/vue-reactivity-project-alstnc`,
        '_blank'
      )
    },
    onClickSite() {
      window.open(`https://rpgcharactergen.netlify.app/`, '_blank')
    },
  },
}
</script>

<style lang="scss"></style>
