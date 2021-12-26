<template>
  <v-app>
    <v-main>
      <Header />
      <Footer />
    </v-main>
  </v-app>
</template>

<script>
import Header from "./components/Layouts/Header";
import Footer from "./components/Layouts/Footer";

export default {
  name: "App",
  components: {
    Header,
    Footer,
  },

  data: () => ({
    //
  }),
};
</script>

<style lang="scss">
html{
  direction: rtl;
}
</style>