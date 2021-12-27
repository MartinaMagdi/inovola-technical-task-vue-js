<template>
  <div class="section-two">
    <div class="right-side">
      <p class="first-text">كل ما تحتاجه لنمو متجرك فى مكان واحد</p>
      <p class="second-text">
        مميزات سوق تطبيقات زد تساعدك فى سهولة وسرعة الاستفادة من خدمات وحلول
      </p>
      <p class="second-text">سوق التطبيقات لنمو متجرك ومضاعفة أرباحك</p>
      <ul class="list-items-container">
        <li class="list-item" v-for="item in listItems" :key="item.id">
          <img class="item-icon" :src="item.icon" :alt="item.alt" />
          <span>{{ item.content }}</span>
        </li>
      </ul>
      <button class="btn">
        <span>تصفح التطبيقات</span>
        <v-icon>mdi-chevron-left</v-icon>
      </button>
    </div>
    <div class="left-side">
      <img
        class="dot-pattern"
        src="../../assets/images/Landing page/Dot-Pattern2.png"
        alt="Dot-Pattern"
      />
      <img
        class="ellipse"
        src="../../assets/images/Landing page/Ellipse.png"
        alt="Ellipse"
      />
      <img
        class="section-img"
        src="../../assets/images/Landing page/Section two/section2-img.png"
        alt="Section image"
      />
    </div>
  </div>
</template>

<script>
import itemOneIcon from "../../assets/images/Landing page/Section two/first-icon.png";
import itemTwoIcon from "../../assets/images/Landing page/Section two/second-icon.png";
import itemThreeIcon from "../../assets/images/Landing page/Section two/third-icon.png";

export default {
  name: "SectionTwo",
  data: () => ({
    listItems: [
      {
        id: 0,
        icon: itemOneIcon,
        alt: "icon",
        content: "سهولة ادارة و تفعيل تطبيقاتك من نفس لوحة تحكم متجرك",
      },
      {
        id: 1,
        icon: itemTwoIcon,
        alt: "icon",
        content: "دعم فنى وتقني متكامل متوفر على مدار الساعة",
      },
      {
        id: 2,
        icon: itemThreeIcon,
        alt: "icon",
        content: "أسعار تنافسية مع تجربة مجانية وباقات اشتراك متنوعة",
      },
    ],
  }),
};
</script>

<style lang="scss" scoped>
@import "../../assets/styles/variables";
@import "../../assets/styles/Landing page/SectionTwo";
</style>