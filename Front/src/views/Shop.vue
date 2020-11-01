<template>
  <div>
    <Header />
    <div class="shop-main">
      <div v-for="prod in product" :key="prod._id" class="shop">
        <img class="img" src="@/assets/img/img.jpg" />
        <div class="txt">
          <hr />
          <h3>Reviews</h3>
          <h3>{{prod.name}}</h3>
          <h4>Rs. {{prod.price}}</h4>
        </div>
      </div>
    </div>
    <Footer />
  </div>
</template>

<script>
import Header from "../components/Layout/Header";
import Footer from "../components/Layout/Footer";
import axios from "axios";
export default {
  components: {
    Header,
    Footer,
  },
  data() {
    return {
      product: [],
    };
  },
  mounted() {
    axios.get("http://localhost:3000/product").then((res) => {
      this.product = res.data;
      console.log(this.product);
    });
  },
};
</script>

<style scoped>
.shop-main {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  max-width: 1200px;
  margin: auto;
  padding: 3% 0;
}
.shop {
  border: 1px solid black;
  max-width: 350px;
  margin-bottom: 40px;
}
.img {
  max-width: 350px;
}
</style>