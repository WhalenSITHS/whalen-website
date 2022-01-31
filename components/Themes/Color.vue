<template>
  <li class="theme-icon" @click="$colorMode.preference = color">
    <span class="icon"><fa :icon="icon" /> </span>
    <span class="color-name">{{ color }}</span>
  </li>
</template>

<script>
export default {
  props: {
    icon: String,
    color: String,
  },
}
</script>

<style lang="scss">
.theme-icon {
  width: 32%;
  font-size: var(--h2);
  color: var(--text-primary);
  list-style: none;
  margin: 2rem auto;
  transition: all 0.3s;
  display: flex;
  align-items: center;
  justify-content: center;
}
@include tablet {
  .theme-icon {
    width: 40%;
  }
}
@include phone {
  .theme-icon {
    width: 90%;
  }
}
.icon,
.color-name {
  margin: 1rem;
  border-bottom: 3px solid transparent;
}
.theme-icon:hover {
  //transform: scale(1.1);

  cursor: pointer;
}
.theme-icon:hover .color-name {
  border-bottom: 3px solid white;
}
</style>
