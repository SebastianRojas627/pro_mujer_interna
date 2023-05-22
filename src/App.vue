<template>
  <NavBar></NavBar>
  <body>
    <CoverImage />
    <PageDescription />
    <WhatWeDo />
    <WhoWeAre />
    <LocationMap />
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
  },
};
</script>

<style>
body {
  padding-top: 2.3rem; /* adjust this value to match the height of your navbar */
}
</style>
