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

    <!--  BrandCommerce  -->
    <BrandCommerce />
    <!--  BrandCommerce  -->
  </div>
</template>

<script>
import CardResume from '@/components/CardResume'
import Education from '@/components/Education'
import CardExperience from '@/components/CardExperience'
import BrandCommerce from '@/components/BrandCommerce'

export default {
  components: { BrandCommerce, CardExperience, Education, CardResume },
  layout: 'resume'
}
</script>
