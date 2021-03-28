<template>
  <div id="CardResume">
    <v-card
      class="mx-auto rounded-xl"
      outlined
    >
      <v-container>
        <v-row no-gutters>
          <v-col
            class="mb-3"
            cols="12"
            sm="6"
            justify="start" align="start"
          >
            <div class="ma-6">
              <div class="mb-10">
                <div class="display-4 font-weight-medium">RESUME</div>
                <div class="display-1 font-weight-light mb-3">JAKARIN MONTHONG</div>
                <div class="display-1 font-weight-light mb-2">ONLINE DESIGN SUPERVISOR</div>
                <div class="display-1 font-weight-light">(Head Of Design Team Lead)</div>
                <div class="display-1" style="color: #52C762;">E-Commerce - Commercial</div>
              </div>

              <div>
                <div class="display-1">092-5165424</div>
                <div class="display-1">myhorus5424@gmail.com</div>
              </div>
            </div>
          </v-col>

          <v-col
            cols="12"
            sm="6"
            justify="center" align="center"
          >
            <v-img
              :lazy-src="require(`~/assets/img/${profileImg}.png`)"
              max-width="361"
              class="rounded-xl position-img-profile"
              :src="require(`~/assets/img/${profileImg}.png`)"
            ></v-img>
          </v-col>
        </v-row>
      </v-container>
    </v-card>
  </div>
</template>

<script>
export default {
  name: 'CardResume',
  data() {
    return {
      profileImg: 'profile'
    }
  }
}
</script>

<style scoped>
.position-img-profile {
  margin: -30px 0px 20px 0px;
}
</style>
