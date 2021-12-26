<template>
  <v-app>
    <v-main>
      <Header />
      <LandingPage />
      <Footer />
    </v-main>
  </v-app>
</template>

<script>
import Header from "./components/Layouts/Header";
import Footer from "./components/Layouts/Footer";
import LandingPage from "./components/Landing page/index.vue"

export default {
  name: "App",
  components: {
    Header,
    Footer,
    LandingPage
  },

  data: () => ({
  }),
};
</script>

<style lang="scss">
html{
  direction: rtl;
}
</style>