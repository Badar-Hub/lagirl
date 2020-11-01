<template>
  <div>
    <div class="main max">
      <div class="main-inner-first max">
        <div class="show">
          <h2>
            SHOW OFF
            <br />YOUR LOOK!
          </h2>
        </div>
        <div class="show">
          <h3>
            <a href="#">#LAGIRLCOSMETICS</a>
          </h3>
        </div>
        <div class="show">
          <img src="@/assets/img/lag.png" />
        </div>
      </div>
      <Slider :swiper-option="swiperOption">
        <template #slider-content>
          <swiper-slide>
            <img src="@/assets/img/Slider/LAG_pretty_and_plump_web_banner_landing_page_1920x.jpg" />
          </swiper-slide>
          <swiper-slide>
            <img
              src="@/assets/img/Slider/LAG_keep_it_playful_web_banner_landing_page_v1_1920x.webp"
            />
          </swiper-slide>
          <swiper-slide>
            <img
              src="@/assets/img/Slider/LAG_Shimmer_Lip_attraction_web_banner_landing_page_v1_1920x.gif"
            />
          </swiper-slide>
          <swiper-slide>
            <img
              src="@/assets/img/Slider/LAG_Shimmer_Lip_attraction_web_banner_landing_page_v1_1920x.gif"
            />
          </swiper-slide>
          <swiper-slide>
            <img
              src="@/assets/img/Slider/LAG_Shimmer_Lip_attraction_web_banner_landing_page_v1_1920x.gif"
            />
          </swiper-slide>
          <swiper-slide>
            <img
              src="@/assets/img/Slider/LAG_Shimmer_Lip_attraction_web_banner_landing_page_v1_1920x.gif"
            />
          </swiper-slide>
          <swiper-slide>
            <img
              src="@/assets/img/Slider/LAG_Shimmer_Lip_attraction_web_banner_landing_page_v1_1920x.gif"
            />
          </swiper-slide>
          <swiper-slide>
            <img
              src="@/assets/img/Slider/LAG_Shimmer_Lip_attraction_web_banner_landing_page_v1_1920x.gif"
            />
          </swiper-slide>
        </template>
      </Slider>
    </div>
  </div>
</template>

<script>
import Slider from "./slider";
export default {
  components: {
    Slider,
  },
  data() {
    return {
      swiperOption: {
        slidesPerView: 4,
        spaceBetween: 30,
        freeMode: true,
        // pagination: {
        //   el: ".swiper-pagination",
        //   type: "progressbar",
        // },
        navigation: {
          nextEl: ".swiper-button-next",
          prevEl: ".swiper-button-prev",
        },
      },
    };
  },
};
</script>

<style scoped>
.main-inner-first {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
}
img {
  max-width: 250px;
  width: 100%;
}
</style>