<template>
  <div class="footer">
    <div>
      <img src="../../assets/images/zid-logo-2.png" alt="logo" />
      <ul class="social-container">
        <li class="social-item">
          <a>
            <v-icon>mdi-twitter</v-icon>
          </a>
        </li>
        <li class="social-item">
          <a>
            <v-icon>mdi-instagram</v-icon>
          </a>
        </li>
        <li class="social-item">
          <a>
            <i class="fab fa-linkedin-in"></i>
          </a>
        </li>
        <li class="social-item">
          <a>
            <v-icon>mdi-youtube</v-icon>
          </a>
        </li>
      </ul>
    </div>
    <div class="buttons-container">
      <v-icon class="message-icon">mdi-forum</v-icon>
      <v-icon class="arrow-icon">mdi-arrow-up</v-icon>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'Footer',

    data: () => ({
    }),
  }
</script>

<style lang="scss" scoped>
@import "../../assets/styles/variables";
@import "../../assets/styles/Layouts/Footer";
</style>
