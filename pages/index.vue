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

    <!--  CardCampaign  -->
    <CardCampaign />
    <!--  CardCampaign  -->
  </div>
</template>

<script>
import CardResume from '@/components/CardResume'
import Education from '@/components/Education'
import CardExperience from '@/components/CardExperience'
import BrandCommerce from '@/components/BrandCommerce'
import CardCampaign from '@/components/CardCampaign'

export default {
  components: { CardCampaign, BrandCommerce, CardExperience, Education, CardResume },
  layout: 'resume'
}
</script>
