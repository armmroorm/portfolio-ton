<template>
  <div id="CardCampaign" class="mb-8">
    <v-card
      class="mx-auto rounded-xl"
      outlined
    >
      <v-container>
        <v-row no-gutters>
          <v-col
            v-for="(item, i) in campaigns"
            :key="i"
            class="mb-5"
            cols="6"
            sm="4"
            md="3"
            justify="start" align="start"
          >
            <div>
              <v-img
                :lazy-src="require(`~/assets/img/${item.img}.png`)"
                max-width="60"
                max-height="80"
                class="mx-auto"
                :src="require(`~/assets/img/${item.img}.png`)"
              ></v-img>
            </div>

            <div class="title text-center">{{ item.subtitle }}</div>
          </v-col>
        </v-row>
      </v-container>
    </v-card>
  </div>
</template>

<script>
export default {
  name: 'CardCampaign',
  data() {
    return {
      campaigns: [
        { img: 'colleg', subtitle: 'Key Visual (All Brand)' },
        { img: 'colleg', subtitle: 'Template Campaign' },
        { img: 'colleg', subtitle: 'Control Brand CI' },
        { img: 'colleg', subtitle: 'Brand (Coordinate)' },
        { img: 'colleg', subtitle: 'Key Approve Brand' },
        { img: 'colleg', subtitle: 'Brand Landing Page' },
        { img: 'colleg', subtitle: 'Brand Banner' },
        { img: 'colleg', subtitle: 'Brand Social Media' },
        { img: 'colleg', subtitle: 'Brand Special Project' },
        { img: 'colleg', subtitle: 'Super Brand Day' },
        { img: 'colleg', subtitle: 'Official Store Channel' },
        { img: 'colleg', subtitle: 'Marketplace Platform' },
        { img: 'colleg', subtitle: '4.4Summer Campaign' },
        { img: 'colleg', subtitle: '9.9Campaign' },
        { img: 'colleg', subtitle: '11.11Campaign' },
        { img: 'colleg', subtitle: '12.12Campaign' }
      ]
    }
  }
}
</script>

<style scoped>

</style>
