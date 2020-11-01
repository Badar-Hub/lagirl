<template>
  <div>
    <Header />
    <div class="eye">
      <div class="text-eye sp">
        <h1>jhnsdkjhfbgsdwehjf</h1>
      </div>
    </div>
    <div class="eye-menu">
      <div class="eye-menu-inner">
        <div class="sub-categories">
          <ul>
            <li>
              <a href="#">EYEBROW</a>
            </li>
            <li>
              <a href="#">EYELINER</a>
            </li>
            <li>
              <a href="#">EYESHADOW</a>
            </li>
            <li>
              <a href="#">MASCARA</a>
            </li>
          </ul>
        </div>
        <div class="sub-categories">
          <ul>
            <li>
              <a href="#">SHOW FILTERS +</a>
            </li>
          </ul>
        </div>
      </div>
    </div>
    <div class="eye-inner">
      <div class="eye-text">
        <h3>37 PRODUCTS</h3>
        <h3>
          SORT BY
          <select style="padding:8px">
            <option>FEATURED</option>
            <option>Price: Low to High</option>
            <option>Price: High to Low</option>
            <option>A-Z</option>
            <option>Oldest To Newest</option>
            <option>Newest To Oldest</option>
            <option>Best Selling</option>
          </select>
        </h3>
      </div>
    </div>
    <Footer />
  </div>
</template>

<script>
import Header from "../components/Layout/Header";
import Footer from "../components/Layout/Footer";
export default {
  components: {
    Header,
    Footer,
  },
};
</script>

<style scoped>
.eye-text {
  display: flex;
  max-width: 1200px;
  justify-content: space-between;
  margin: auto;
}
.eye-menu {
  background-color: #383838;
}
.eye-menu-inner {
  display: flex;
  justify-content: space-between;
  max-width: 1200px;
  margin: auto;
}
.sub-categories ul {
  display: flex;
  max-width: 1200px;
  margin: 0 auto;
  list-style-type: none;
  padding: 20px;
}

.sub-categories ul li {
}

.sub-categories ul li a {
  color: white;
  padding-right: 20px;
  text-decoration: none;
}
.eye {
  background-image: url("../assets/img/Categories/Eye.jpg");
  height: 200px;
}
.sp {
  display: flex;
  max-width: 1200px;
  flex-direction: column;
  margin: auto;
  justify-content: center;
}
</style>