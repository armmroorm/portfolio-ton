<template>
  <div>
    <!--   Card Resume   -->
    <CardResume />
    <!--   Card Resume   -->

    <!-- Education -->
    <Education />
    <!-- Education -->

    <!--  Experience  -->
    <CardExperience />
    <!--  Experience  -->
  </div>
</template>

<script>
import CardResume from '@/components/CardResume'
import Education from '@/components/Education'
import CardExperience from '@/components/CardExperience'

export default {
  components: { CardExperience, Education, CardResume },
  layout: 'resume'
}
</script>
