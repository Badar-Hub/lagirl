<template>
  <div>
    <Header />
    <Slider :swiper-option="swiperOption">
      <template #slider-content>
        <swiper-slide>
          <img src="@/assets/img/Slider/LAG_pretty_and_plump_web_banner_landing_page_1920x.jpg" />
        </swiper-slide>
        <swiper-slide>
          <img src="@/assets/img/Slider/LAG_keep_it_playful_web_banner_landing_page_v1_1920x.webp" />
        </swiper-slide>
        <swiper-slide>
          <img
            src="@/assets/img/Slider/LAG_Shimmer_Lip_attraction_web_banner_landing_page_v1_1920x.gif"
          />
        </swiper-slide>
      </template>
    </Slider>
    <div class="Bcolor">
      <div class="max">
        <img src="@/assets/img/Slider/LAG_break_free_Homepage_video_1_2400x.gif" />
      </div>
    </div>
    <overlayCategory style="background-color:#eb008b30" />
    <Footer />
  </div>
</template>

<script>
import Header from "../components/Layout/Header";
import Slider from "../components/slider";
import overlayCategory from "../components/overlayCategory";
import Footer from "../components/Layout/Footer";

export default {
  name: "App",

  components: {
    Header,
    Slider,
    overlayCategory,
    Footer,
  },
  data() {
    return {
      swiperOption: {
        slidesPerView: 1,
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
body {
  margin: 0;
  padding: 0;
}

a {
  font-family: Lato;
}

.Bcolor {
  background-color: black;
  color: white;
}

.max {
  padding: 3% 0;
  max-width: 1200px;
  margin: auto;
}

img {
  width: 100%;
  height: auto;
}
</style>
