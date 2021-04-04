<template>
  <div class="mb-12">
    <VueSlickCarousel v-bind="settings">
      <slot></slot>
    </VueSlickCarousel>
  </div>
</template>

<script>

export default {
  name: 'Carousel',
  props: {
    settings: {
      type: [Object, Array],
      default() {
        return {
          'dots': true,
          'focusOnSelect': true,
          'infinite': true,
        }
      }
    }
  },
  data() {
    return {}
  }
}
</script>

<style scoped>
</style>
