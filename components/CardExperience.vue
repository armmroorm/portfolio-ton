<template>
  <div id="CardExperience">
    <v-card
      class="mx-auto rounded-xl pa-6"
      outlined
    >
      <v-container>
        <!--  TimeExperience  -->
        <TimeExperience />

        <!--  CompanyEnvironment  -->
        <CompanyEnvironment />
      </v-container>
    </v-card>
  </div>
</template>

<script>
import TimeExperience from '@/components/TimeExperience'
import CompanyEnvironment from '@/components/CompanyEnvironment'

export default {
  name: 'CardExperience',
  components: { CompanyEnvironment, TimeExperience }
}
</script>

<style scoped>

</style>
