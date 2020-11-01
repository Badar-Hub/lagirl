<template>
  <div class="Bcolor">
    <div class="footer">
      <div class="inner">
        <h3>CUSTOMER SERVICE</h3>
        <p>MY ACCOUNT</p>
        <p>FIND A STORE</p>
        <p>CAREERS</p>
        <p>ABOUT US</p>
        <br />
        <h3>FOLLOW US</h3>
        <span>
          <a href="#">
            <img class="social-icons" src="@/assets/img/Social/instagram.svg" />
          </a>
          <a href="#">
            <img class="social-icons" src="@/assets/img/Social/facebook.svg" />
          </a>
          <a href="#">
            <img class="social-icons" src="@/assets/img/Social/twitter.svg" />
          </a>
          <a href="#">
            <img class="social-icons" src="@/assets/img/Social/youtube.svg" />
          </a>
        </span>
      </div>
      <div class="inner">
        <h3 style="color:black">.</h3>
        <p>FAQ</p>
        <p>SHIPPING POLICY</p>
        <p>RETURN POLICY</p>
        <p>CONTACT US</p>
        <br />
        <img class="bunny" src="@/assets/img/Social/crueltyfree_bunny.webp" />
      </div>
      <div class="inner">
        <img class="cosmetic-slogan" src="@/assets/img/Social/LAG_cosmetics_slogan.svg" />
        <br />
        <p>SIGN UP FOR OUR LATEST PROMOTIONS AND DEALS.</p>
        <input style="width:100%; height:25px" type="text" placeholder="Enter your email" />
        <br />
        <button>SUBSCRIBE</button>
        <br />
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.footer {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
  max-width: 1200px;
  margin: auto;
}
.bunny {
  max-width: 90px;
  width: 100%;
}
.social-icons {
  max-width: 40px;
  padding-right: 10px;
}
.cosmetic-slogan {
  width: 100%;
  padding: 3%;
}
button {
  width: 100%;
  margin-top: 10px;
  font-size: 1.3rem;
  padding: 5px;
  background-color: #eb0089;
  border: none;
}
</style>