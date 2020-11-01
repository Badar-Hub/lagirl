<template>
  <div>
    <Header />
    <!-- <div class="category-title">
      <p>Home</p>
      <p>Home</p>
      <p>Home</p>
    </div>-->
    <div v-for="prod in product" :key="prod._id" class="product-info">
      <div class="main">
        <div class="prod-info">
          <img style="max-width:500px;" src="../assets/img/img.jpg" />
        </div>
        <div class="prod-infos">
          <div>
            <h3>{{prod.name}}</h3>
            <h3>reviews</h3>
            <h3>Rs. {{prod.price}}</h3>
            <hr />
            <h4>SELECTED SHADE: GBG381 Dark Blonde</h4>
            <select style="width:80%; padding:10px;">
              <option>Select Shade</option>
              <option>GBG381 Dark Blonde 1</option>
              <option>GBG382 Dark Blonde 2</option>
              <option>GBG383 Dark Blonde 3</option>
              <option>GBG384 Dark Blonde 4</option>
              <option>GBG385 Dark Blonde 5</option>
            </select>
            <select style="width:20%; padding:10px;">
              <option>1</option>
              <option>2</option>
              <option>3</option>
              <option>4</option>
              <option>5</option>
              <option>6</option>
              <option>7</option>
              <option>8</option>
              <option>9</option>
              <option>10</option>
            </select>
            <br />
            <button class="shop">ADD TO BAG</button>
            <h4>FREE SHIPPING ON ORDERS OVER $35</h4>
          </div>
        </div>
      </div>
      <div class="main mains">
        <div class="prod-info">
          <hr style="margin:0" />
          <h3>YOU MAY ALSO LIKE</h3>
          <div class="related-product">
            <div class="prod">
              <img class="img" src="@/assets/img/img2.jpg" />
              <p>
                Brow Bestie
                <br />Triangular Auto
                <br />Pencil
              </p>
            </div>
            <div class="prod">
              <img class="img" src="@/assets/img/img2.jpg" />
              <p>
                Brow Bestie
                <br />Triangular Auto
                <br />Pencil
              </p>
            </div>
            <div class="prod">
              <img class="img" src="@/assets/img/img2.jpg" />
              <p>
                Brow Bestie
                <br />Triangular Auto
                <br />Pencil
              </p>
            </div>
          </div>
        </div>
        <div class="description">
          <button class="btn">DESCRIPTION</button>
          <!-- <h3 style="border:1px solid black">Description</h3> -->
          <hr style="margin:0" />
          <p>
            <strong>PRODUCT DESCRIPTION</strong>
          </p>
          <p style="line-height:1.5">{{prod.description}}</p>
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
.main {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(500px, 1fr));
  max-width: 1200px;
  margin: auto;
  text-align: left;
  padding-bottom: 2%;
}

.mains {
  padding-bottom: 6%;
}

.shop {
  width: 100%;
  color: white;
  background-color: #eb008b;
  padding: 10px;
  margin-top: 10px;
}
img {
  width: 100%;
}

.prod-info {
  margin: auto;
}

.prod-infos {
  display: flex;
  flex-direction: column;
  justify-content: center;
}
h3 {
  font-size: 24px;
  text-transform: uppercase;
}

.related-product {
  display: flex;
  flex-wrap: wrap;
  text-align: center;
}

.prod {
  padding-right: 20px;
}

.img {
  border: 1px solid rgba(0, 0, 0, 0.267);
  max-width: 160px;
}

.category-title {
  display: flex;
  flex-wrap: wrap;
  max-width: 1200px;
  margin: auto;
}

.btn {
  background-color: #4caf50; /* Green */
  border: none;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
}
</style>