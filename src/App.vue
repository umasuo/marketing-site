<template>
  <div id="app">

    <Navbar></Navbar>

    <HeaderSection></HeaderSection>

    <GuideSection></GuideSection>

    <FeaturesWithImgSection></FeaturesWithImgSection>

    <Download></Download>

    <FeaturesSection></FeaturesSection>

    <GetStartedSection></GetStartedSection>

    <SocialSection></SocialSection>

    <Footerbar></Footerbar>
  </div>
</template>

<script>
  import Navbar from './components/Navbar.vue'
  import HeaderSection from './components/HeaderSection.vue'
  import Download from './components/DownloadSection.vue'
  import FeaturesSection from './components/FeaturesSection.vue'
  import GetStartedSection from './components/GetStartedSection.vue'
  import SocialSection from './components/SocialSection.vue'
  import Footerbar from './components/Footerbar.vue'
  import FeaturesWithImgSection from './components/FeaturesWithImgSection.vue'
  import GuideSection from './components/GuideSection.vue'

  export default {
    name: 'app',
    components: {
      Navbar,
      HeaderSection,
      Download,
      FeaturesSection,
      GetStartedSection,
      SocialSection,
      Footerbar,
      FeaturesWithImgSection,
      GuideSection
    }
  }
</script>

<style lang="scss">
  @import '~src/scss/style';
</style>
