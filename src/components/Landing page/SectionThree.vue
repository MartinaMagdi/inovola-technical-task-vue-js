<template>
  <div class="section-three">
    <p class="first-text">التطبيقات المميزة</p>
    <p class="second-text">تطبيقات تقدم حلول وخدمات مميزة نوصي بتجربتها</p>

    <div class="features-apps-container">
      <div class="item" v-for="item in featuredAppsList" :key="item.id">
        <div class="right-side">
          <img :src="item.img" :alt="item.altImg" />
        </div>
        <div class="left-side">
          <div class="title-container">
            <p class="card-title">{{ item.name }}</p>
            <span><v-icon>mdi-star</v-icon> {{ item.starNum }}</span>
          </div>
          <p class="developer-name">
            تطوير: <span>{{ item.developerName }}</span>
          </p>
          <p class="description">{{ item.firstDes }}</p>
          <p class="description">{{ item.secondDes }}</p>
        </div>
      </div>
    </div>

    <button class="btn">
      <span>جميع التطبيقات</span>
      <v-icon>mdi-chevron-left</v-icon>
    </button>
  </div>
</template>

<script>
import cardImage from "../../assets/images/Landing page/section3-img.png";

export default {
  name: "SectionThree",
  data: () => ({
    featuredAppsList: [
      {
        id: 0,
        img: cardImage,
        altImg: "logo",
        name: "قمرة",
        starNum: 5,
        developerName: "عمر برهوم",
        firstDes: "نظام الولاء الأمثل الذي يمكنك من رفع مبيعاتك",
        secondDes: "نظام الولاء الأمثل الذي يمكنك من رفع مبيعاتك",
      },
      {
        id: 1,
        img: cardImage,
        altImg: "logo",
        name: "قمرة",
        starNum: 5,
        developerName: "عمر برهوم",
        firstDes: "نظام الولاء الأمثل الذي يمكنك من رفع مبيعاتك",
        secondDes: "نظام الولاء الأمثل الذي يمكنك من رفع مبيعاتك",
      },
      {
        id: 2,
        img: cardImage,
        altImg: "logo",
        name: "قمرة",
        starNum: 5,
        developerName: "عمر برهوم",
        firstDes: "نظام الولاء الأمثل الذي يمكنك من رفع مبيعاتك",
        secondDes: "نظام الولاء الأمثل الذي يمكنك من رفع مبيعاتك",
      },
      {
        id: 3,
        img: cardImage,
        altImg: "logo",
        name: "قمرة",
        starNum: 5,
        developerName: "عمر برهوم",
        firstDes: "نظام الولاء الأمثل الذي يمكنك من رفع مبيعاتك",
        secondDes: "نظام الولاء الأمثل الذي يمكنك من رفع مبيعاتك",
      },
    ],
  }),
};
</script>

<style lang="scss" scoped>
@import "../../assets/styles/variables";
@import "../../assets/styles/Landing page/SectionThree";
</style>