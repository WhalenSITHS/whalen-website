<template>
  <div>
    <prismic-rich-text class="textslice" :field="slice.primary.text" />
  </div>
</template>

<script>
export default {
  props: ['slice'],
  name: 'text-slice',
}
</script>

<style lang="scss">
.textslice {
  text-align: left;
}
p a,
p a:link,
p a:visited {
  color: #fff;
}
</style>
