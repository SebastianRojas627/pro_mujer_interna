<template>
  <NavBar></NavBar>
  <body>
    <CoverImage />
    <PageDescription />
    <WhatWeDo />
    <WhoWeAre />
    <LocationMap />
    <OurAchievements />
    <StorySection />
    <Informes />
  </body>
  <Footer></Footer>
</template>

<script>
import NavBar from "./components/NavBar.vue";
import WhatWeDo from "./components/WhatWeDo.vue";
import CoverImage from "./components/CoverImage.vue";
import Informes from "./components/Informes.vue";
import Footer from "./components/Footer.vue";
import PageDescription from "./components/PageDescription.vue";
import WhoWeAre from "./components/WhoWeAre.vue";
import LocationMap from "./components/LocationMap.vue";
import OurAchievements from "./components/OurAchievements.vue";
import StorySection from "./components/StorySection.vue";

export default {
  name: "App",
  components: {
    NavBar,
    WhatWeDo,
    CoverImage,
    Informes,
    Footer,
    PageDescription,
    WhoWeAre,
    LocationMap,
    OurAchievements,
    StorySection,
  },
};
</script>

<style>
body {
  padding-top: 2.3rem;
}
</style>
