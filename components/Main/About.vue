<template>
  <section class="about">
    <h2 class="about-header">About Us</h2>
    <div class="about-content">
      <div class="about-card">
        <span class="icon about-icon"><fa icon="low-vision" /></span>
        <h3 class="about-card-header">Accessibility</h3>
        <hr class="card-rule" />
        <p class="about-text-content">
          Starting in 2020-2021, we have implemented a focus on accessibility to
          empower our students to consider all of our users and create
          accessible content
        </p>
      </div>
      <div class="about-card">
        <span class="icon about-icon"><fa icon="code-branch" /></span>
        <h3 class="about-card-header">Version Control</h3>
        <hr class="card-rule" />
        <p class="about-text-content">
          Students are introduced to Git immediately and utilize it’s full
          functionality to collaborate and ensure version control
        </p>
      </div>
      <div class="about-card">
        <span class="icon about-icon"><fa icon="users" /></span>
        <h3 class="about-card-header">Student Agency</h3>
        <hr class="card-rule" />
        <p class="about-text-content">
          Students are encouraged to be creative and make their own choices
          regarding their projects
        </p>
      </div>
      <div class="about-card">
        <span class="icon about-icon"><fa icon="database" /></span>
        <h3 class="about-card-header">Real Skills</h3>
        <hr class="card-rule" />
        <p class="about-text-content">
          The curriculum and projects are designed to blur the lines between
          high school and the current paradigms in development
        </p>
      </div>
    </div>
  </section>
</template>

<script>
export default {}
</script>

<style lang="scss">
.about {
  height: 90vh;
  width: 90vw;
  margin: 0 auto;
}
.about-header {
  margin: 5rem auto;
  text-transform: uppercase;
  font-size: var(--h1);
}
.about-content {
  margin: 10rem auto;
  display: flex;
  justify-content: space-around;
  align-items: center;
}

.about-card {
  border-radius: 2rem;
  padding: 2rem;
  width: 20%;
  display: flex;
  flex-direction: column;
  align-items: center;
  box-shadow: var(--level-2);
  height: 55vh;
  text-align: center;
  background-color: var(--card-background);
  color: var(--card-text);
  transition: all 0.3s;
}

.about-card:hover {
  transform: translateY(-10px);
}
.card-rule {
  width: 90%;
  margin: 2.5% auto;
  color: var(--card-rule);
}
.about-icon {
  font-size: var(--h2);
  margin: 5%;
}
.about-card-header {
  margin: 2.5% auto;
  font-style: italic;
}
.about-text-content {
  font-size: var(--h4);
  margin-top: 10%;
}
@include laptop {
  .about {
    height: 99vh;
  }
  .about-card {
    height: 65vh;
  }
}
@include tablet {
  .about-header {
    margin: rem auto;
  }
  .about-content {
    margin: 4rem auto;
    flex-direction: column;
  }
  .about-card {
    width: 70%;
    height: auto;
    margin: 2rem auto;
    padding: 3rem;
  }
  .about {
    height: auto;
  }
}
@include phone {
  .about-content {
    margin: 2rem auto;
  }
}
</style>
