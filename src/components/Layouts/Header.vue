<template>
  <div class="header">
    <img class="logo-img" src="../../assets/images/zid-logo.png" alt="logo" />
    <div class="header-items-container" v-bind:class="{ headerItemsContainerMobile: menuISOpen }">
      <ul>
        <li class="header-item" v-for="item in headerItems" :key="item.id">
          {{ item.name }}
        </li>
      </ul>
    </div>
    <v-icon class="menu-icons open-menu-icon" v-if="!menuISOpen" @click="toggleMenu()"
      >mdi-menu</v-icon
    >
    <v-icon class="menu-icons close-menu-icon" v-else @click="toggleMenu()"
      >mdi-close</v-icon
    >
  </div>
</template>

<script>
export default {
  name: "Header",

  data: () => ({
    headerItems: [
      {
        id: 0,
        name: "الرئيسية",
        routerLink: "",
      },
      {
        id: 1,
        name: "التصنيفات",
        routerLink: "",
      },
      {
        id: 3,
        name: "التطبيقات",
        routerLink: "",
      },
      {
        id: 4,
        name: "طور تطبيق",
        routerLink: "",
      },
    ],
    menuISOpen: false,
  }),

  methods: {
    toggleMenu() {
        this.menuISOpen = !this.menuISOpen
    },
  },
};
</script>

<style lang="scss" scoped>
@import "../../assets/styles/Layouts/Header.scss";
</style>