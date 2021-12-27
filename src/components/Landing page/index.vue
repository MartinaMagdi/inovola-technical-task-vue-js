<template>
  <div class="landing-page">
    <SectionOne />
    <SectionTwo />
  </div>
</template>

<script>
import SectionOne from "./SectionOne.vue";
import SectionTwo from "./SectionTwo.vue";

export default {
  name: "LandingPage",
  components: { SectionOne, SectionTwo },
};
</script>