<template>
  <slide-carousel>
    <div v-for="(item, i) in educations" :key="i">
      <v-card
        class="mx-auto rounded-xl pa-5"
        max-width="800"
        outlined
      >
        <v-list-item three-line>
          <v-img
            :lazy-src="require(`~/assets/img/${item.img}.png`)"
            max-width="200"
            class="rounded-xl position-img-profile"
            :src="require(`~/assets/img/${item.img}.png`)"
          ></v-img>

          <v-list-item-content>
            <div class="display-1 mb-4">
              {{ item.title }}
            </div>
            <v-list-item-title class="headline mb-1">
              {{ item.subtitle }}
            </v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-card>
    </div>
  </slide-carousel>
</template>

<script>
export default {
  name: 'CardEducation',
  data() {
    return {
      educations: [
        {
          img: 'KMUTT',
          title: 'King Mongkut\'s University Of Technology Thonburi',
          subtitle: 'Applied Computer Science - Multimedia'
        },
        {
          img: 'taweta',
          title: 'Taweethapisek School',
          subtitle: 'Science - Math'
        }
      ]
    }
  }
}
</script>

<style scoped>

</style>
