<template>
  <div>
    <h4 class="block-quotation">
      {{ $prismic.asText(slice.primary.quote) }}
    </h4>
  </div>
</template>

<script>
export default {
  props: ['slice'],
  name: 'quote-slice',
}
</script>

<style lang="scss">
.block-quotation {
  margin: 5rem auto;
  font-size: var(--h3);
  width: 60vw;
}
@media screen and (max-width: 768px) {
  .block-quotation {
    margin: 3rem auto;
    font-size: var(--h4);
    width: 90vw;
  }
}
</style>
