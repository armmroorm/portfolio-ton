<template>
  <slide-carousel :settings="settings">
    <div v-for="item in items" class="text-center px-4">
      <v-card
        class="rounded-pill mb-6"
        outlined
      >
        <v-img
          :lazy-src="require(`~/assets/img/${item.img}.png`)"
          max-width="250"
          max-height="150"
          class="mx-auto "
          :src="require(`~/assets/img/${item.img}.png`)"
        ></v-img>
      </v-card>

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
        { img: 'thisshop', title: 'This shop', subtitle: 'Jr.Designer' },
        { img: 'thisshop', title: 'This shop', subtitle: 'Jr.Designer' },
        { img: 'thisshop', title: 'This shop', subtitle: 'Jr.Designer' },
        { img: 'thisshop', title: 'This shop', subtitle: 'Jr.Designer' },
        { img: 'thisshop', title: 'This shop', subtitle: 'Jr.Designer' }
      ],
      settings: {
        'dots': true,
        'infinite': true,
        'speed': 500,
        'slidesToShow': 4,
        'slidesToScroll': 4,
        'initialSlide': 0,
        'responsive': [
          {
            'breakpoint': 1024,
            'settings': {
              'slidesToShow': 3,
              'slidesToScroll': 3,
              'infinite': true,
              'dots': true
            }
          },
          {
            'breakpoint': 600,
            'settings': {
              'slidesToShow': 2,
              'slidesToScroll': 2,
              'initialSlide': 2
            }
          },
          {
            'breakpoint': 480,
            'settings': {
              'slidesToShow': 1,
              'slidesToScroll': 1
            }
          }
        ]
      }
    }
  }
}
</script>

<style scoped>

</style>
