<template>
  <TopBar></TopBar>
  <body>
    <div><TextComponent></TextComponent></div>
    <div><Component1></Component1></div>
    <div><Informes></Informes></div>
  </body>
  <Footer></Footer>
</template>

<script>
import TopBar from './components/TopBar.vue'
import Component1 from './components/Component1.vue'
import TextComponent from './components/TextComponent.vue'
import Informes from './components/Informes.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    TopBar,
    Component1,
    TextComponent,
    Informes,
    Footer
  }
}
</script>

<style>
body {
  padding-top: 2.5rem; /* adjust this value to match the height of your navbar */
}
</style>
