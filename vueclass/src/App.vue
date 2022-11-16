<template>
  <div>
    <HeaderLayout fonts="nexon" />
    <SliderSection />
    <ImageSection attr="section nexon " layout="container" />
    <ImgTextSection attr="section nexon " layout="container" />
    <CardSection attr="section nexon " layout="container" />
    <TextSection attr="section nexon " layout="container" />
    <BannerSection />
    <FooterLayout attr="section nexon " layout="container" />
  </div>
</template>

<script>
import HeaderLayout from "./components/layout/layout/HeaderLayout.vue";
import SliderSection from "./components/layout/section/SliderSection";
import ImageSection from "./components/layout/section/ImageSection.vue";
import ImgTextSection from "./components/layout/section/ImgTextSection.vue";
import CardSection from "./components/layout/section/CardSection.vue";
import TextSection from "./components/layout/section/TextSection.vue";
import FooterLayout from "./components/layout/layout/FooterLayout.vue";
import BannerSection from "./components/layout/section/BannerSection.vue";

export default {
  name: "App",
  components: {
    HeaderLayout,
    BannerSection,
    SliderSection,
    ImageSection,
    ImgTextSection,
    CardSection,
    TextSection,
    FooterLayout,
  },
};
</script>
