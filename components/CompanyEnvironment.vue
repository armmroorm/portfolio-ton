<template>
  <div id="CompanyEnvironment">
    <div class="text-center mb-4">
      <span class="title font-weight-black">Company Environment</span>
    </div>

    <div class="d-flex justify-space-between">
      <div class="box-company" v-for="item in items">
        <v-chip
          class="d-block text-center mb-8"
          color="green"
          text-color="white"
          large
        >
          <span class="title font-weight-black">{{ item.per }}</span>
        </v-chip>

        <div class="title">{{ item.subtitle }}</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'CompanyEnvironment',
  data() {
    return {
      items: [
        { per: '100%', subtitle: 'Commercial' },
        { per: '100%', subtitle: 'E-Commerce' },
        { per: '100%', subtitle: 'Corporate Retail' }
      ]
    }
  }
}
</script>

<style scoped>
.box-company {
  width: 250px;
  text-align: center;
}
</style>
