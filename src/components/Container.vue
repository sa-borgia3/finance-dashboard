<template>
  <div class="container" :class="{ 'container--small': small }">
    <slot></slot>
  </div>
</template>

<script>
  export default {
    props: {
      small: {
        type: Boolean,
        default: false,
      },
    },
  };
</script>

<style lang="sass" scoped>


  .container
      width: 100%
      // display: flex
      // align-items: center
      margin: 0 auto

      &--small
        width: 80%
        margin: auto
</style>
