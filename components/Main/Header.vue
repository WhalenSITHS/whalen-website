<template>
  <header>
    <div class="heading">
      <div class="overlay"></div>
      <img
        class="heading-img"
        src="https://res.cloudinary.com/dbopxlpuy/image/upload/c_fit,f_auto,q_auto,w_1920/v1611365531/Bao/test_c6zrj6.png"
        alt="Picture of Three Iphones"
      />
      <div class="heading-box">
        <h1>Michael Whalen</h1>
        <h4>Full-Stack Educator</h4>
        <h4>Staten Island Technical High School</h4>
      </div>
    </div>
    <!-- <button class="header-btn btn">
      <nuxt-link to="StudentWork" class="header-btn-link"
        >See Our Work</nuxt-link
      >
    </button> -->
  </header>
</template>

<script>
export default {}
</script>

<style lang="scss">
header {
  height: 100vh;

  background-size: cover;
  background-position: center;
  clip-path: polygon(0 0, 100% 0%, 100% 87%, 0% 100%);
  h1 {
    text-transform: uppercase;
  }
}
/* @include tablet {
  header {
    //background-position: center;
    background-image: url('https://res.cloudinary.com/dbopxlpuy/image/upload/b_rgb:000000,c_scale,f_auto,o_19,w_1920/v1611365531/Bao/test_c6zrj6.png');
  }
} */

.heading {
  text-align: center;

  color: #fff;
}
.overlay {
  position: absolute;
  z-index: 0;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
  background-color: var(--header-overlay);
}
.heading-img {
  z-index: 1;
  position: absolute;
  filter: blur(0px) brightness(0.4);
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
}
.heading-box {
  z-index: 2;
  position: absolute;
  padding: 50px;
  border-radius: 10px;
  top: 40%;
  left: 50%;

  transform: translate(-50%, -50%);
}
.header-btn {
  z-index: 3;
  position: absolute;
  top: 80%;
  left: 50%;
  transform: translate(-50%, -50%);
  font-size: var(--h4);
  height: 5rem;
  color: var(--white);
  border: 1px solid #fff;
  padding: 0.5rem 2.4rem;
  text-decoration: none;
  transition: all 0.4s;
  background-color: transparent;
  border-radius: 3rem;
  transition: all 0.3s;
}
.header-btn:hover {
  border: 1px solid transparent;
  background-color: var(--background-primary);
  cursor: pointer;
  color: var(--header-btn);
  transform: translate(-50%, -60%);
  box-shadow: var(--level-2-white);
}

.header-btn-link,
.header-btn-link:visited,
.header-btn-link:link {
  text-decoration: none;
  color: inherit;
}
</style>
