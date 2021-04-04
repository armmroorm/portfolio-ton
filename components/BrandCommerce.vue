<template>
  <slide-carousel :settings="settings">
    <div v-for="item in items" class="text-center justify-center">
      <v-img
        :lazy-src="require(`~/assets/img/${item.img}.png`)"
        max-width="250"
        max-height="150"
        class="mb-4"
        :src="require(`~/assets/img/${item.img}.png`)"
      ></v-img>

      <div class="title">{{ item.title }}</div>
      <div class="subtitle">{{ item.subtitle }}</div>
    </div>
  </slide-carousel>
</template>

<script>
export default {
  name: 'BrandCommerce',
  data() {
    return {
      items: [
        { img: 'KMUTT', title: 'Oppo', subtitle: 'Jr.Designer' }
      ],
      settings: {
        'dots': true,
        'focusOnSelect': true,
        'infinite': true,
        'speed': 500,
        'slidesToShow': 3,
        'slidesToScroll': 3,
        'touchThreshold': 5
      }
    }
  }
}
</script>

<style scoped>

</style>
