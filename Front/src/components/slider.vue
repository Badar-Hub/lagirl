<template>
  <swiper class="swiper" :options="swiperOption">
    <slot name="slider-content"></slot>
    <div class="swiper-pagination" slot="pagination"></div>
    <div class="swiper-button-prev" slot="button-prev"></div>
    <div class="swiper-button-next" slot="button-next"></div>
  </swiper>
</template>

<script>
export default {
  name: "swiper-example-free-mode",
  title: "Free mode / No fixed positions",
  props: {
    swiperOption: {
      type: Object,
    },
  },
  computed: {},
  mounted() {},
};
</script>

<style lang="scss" scoped>
@import "./base.scss";
</style>