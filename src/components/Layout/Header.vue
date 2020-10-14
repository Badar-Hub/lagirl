<template>
  <div class="main">
    <div class="main-bar">
      <img style="max-width:200px" src="@/assets/img/logo.png" />
      <div class="navbar">
        <ul>
          <li>
            <a @mouseover="mouseOver" href="#">Products</a>
          </li>
          <li>
            <a href="#">What's New</a>
          </li>
          <li>
            <a href="#">Our Stores</a>
          </li>
          <li>
            <a href="#">Contact</a>
          </li>
        </ul>
      </div>
      <div class="navbar">
        <ul>
          <li>
            <a href="#">Sign In</a>
          </li>
          <li>
            <a href="#">Sign Up</a>
          </li>
          <li>
            <a href="#">
              <img style="max-width:20px" src="@/assets/img/cart.png" alt />
            </a>
          </li>
          <li>
            <a href="#">
              <img style="max-width:20px" src="@/assets/img/search.png" alt />
            </a>
          </li>
        </ul>
      </div>
    </div>
    <subBar v-show="active" style="color:white" />
  </div>
</template>

<script>
import subBar from "./sub-bar";
export default {
  data() {
    return {
      active: false,
    };
  },
  components: {
    subBar,
  },
  methods: {
    mouseOver: function () {
      this.active = !this.active;
    },
  },
};
</script>

<style scoped>
.main {
  background-color: black;
}
.main-bar {
  display: flex;
  max-width: 1200px;
  justify-content: space-between;
  margin: auto;
}

.navbar {
  display: flex;
}

.login {
  display: flex;
}
.span {
  margin: auto;
  color: white;
}

ul {
  display: flex;
  list-style-type: none;
  margin: 0;
}

li {
  display: block;
  margin: auto;
}

a {
  font-size: 1rem;
  color: white;
  text-decoration: none;
  padding: 0 1.3rem;
  margin: auto;
  text-transform: uppercase;
  font-weight: bold;
}

a:hover {
  text-decoration: underline;
}
</style>