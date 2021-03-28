<template>
  <div>
    <!--   Card Resume   -->
    <CardResume />
    <!--   Card Resume   -->
    <!-- Education -->
    <Education />
    <!-- Education -->
  </div>
</template>

<script>
import CardResume from '@/components/CardResume'
import Education from '@/components/Education'

export default {
  components: { Education, CardResume },
  layout: 'resume'
}
</script>
