<template>
  <div class="landing-page">
    <SectionOne />
    <SectionTwo />
    <SectionThree />
  </div>
</template>

<script>
import SectionOne from "./SectionOne.vue";
import SectionTwo from "./SectionTwo.vue";
import SectionThree from "./SectionThree.vue";

export default {
  name: "LandingPage",
  components: { SectionOne, SectionTwo, SectionThree },
};
</script>