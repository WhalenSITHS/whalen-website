<template>
  <div @click="makeHidden" class="modal-container">
    <h2 class="modal-header">CSS Design Systems and Accessibility</h2>
    <div class="modal-flex-row">
      <div class="modal-flex-col">
        <img
          src="https://res.cloudinary.com/dbopxlpuy/image/upload/c_scale,f_auto,w_300/v1613094438/Logos/Sass_Logo_Color_r1mv6v.png"
          alt="SCSS Logo "
          class="modal-logo"
        />
        <p class="modal-text-content">
          Starting in 2020-2021, we began our "Accessibility in Design"
          initiative. Students in the first year Computer Science and
          Engineering course learn about accessable design and best practices
          while learning the fundamentals of CSS. Students are taught to build
          out a full CSS design system while leveraging the power of CSS custom
          properties, SCSS mix-ins and SCSS nesting to ensure all users can
          navigate our applications.
        </p>
      </div>
      <!-- <div class="modal-flex-col">
        <img
          class="modal-image"
          src="https://res.cloudinary.com/dbopxlpuy/image/upload/c_scale,f_auto,w_800/v1613337501/Fantasy Kingdom/Screenshot_2021-02-11_Galgudd_rfkjts.png"
          alt="Blackjack game developed by Nick Melkadze"
        />
      </div> -->
    </div>
    <button class="modal-btn btn">Close</button>
  </div>
</template>

<script>
export default {
  props: ['SCSS'],

  methods: {
    makeHidden: function () {
      this.$emit('hide')
    },
  },
}
</script>

<style lang="scss">
.modal-container {
  background-color: var(--modal-background);
  margin: 0 auto;
  color: var(--modal-text);
  height: 100%;
  width: 80%;
  text-align: center;
  z-index: 3;
}
.modal-header {
  text-transform: uppercase;
  margin: 3rem auto;
}
.modal-flex-row {
  @include flex-row;
  justify-content: space-around;
  width: 90%;
  margin: 10rem auto;
}
.modal-flex-col {
  @include flex-col;
  width: 40%;
  justify-content: space-around;
}
.modal-logo {
  width: 30%;
}
.modal-image {
  width: 100%;
}
.modal-text-content {
  margin-top: 10rem;
  font-size: var(--h4);
  padding: 1rem;
  text-align: left;
}
@include tablet {
  .modal-header {
    font-size: var(--h3);
  }
  .modal-container {
    background-color: black;
    margin: 0 auto;
    color: #fff;
    height: auto;
    width: 85%;
    padding: 1rem;
    text-align: center;
    z-index: 3;
  }
  .modal-flex-row {
    flex-direction: column;
    height: auto;
    width: 100%;
    margin: 3rem auto;
  }
  .modal-flex-col {
    width: 90%;
  }
  .modal-image {
    width: 50%;
  }
  .modal-logo {
    width: 20%;
  }
  .modal-text-content {
    margin: 2rem auto;
    text-align: center;
  }
}
</style>
