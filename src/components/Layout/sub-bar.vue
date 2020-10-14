<template>
  <div>
    <div class="main">
      <div class="main-txt">
        <h2>EYES</h2>
        <p>EYEBROW</p>
        <p>EYELINER</p>
        <p>EYESHADOW</p>
        <p>MASCARA</p>
        <h2>NAILS</h2>
        <p>POLISH</p>
        <p>TREATMENT</p>
      </div>
      <div class="main-txt">
        <h2>LIPS</h2>
        <p>LIP CARE</p>
        <p>LIPGLOSS</p>
        <p>LIPLINER</p>
        <p>LIPSTICK</p>
        <h2>ACCESSORIES</h2>
        <p>BRUSHES</p>
        <p>TOOLS</p>
      </div>
      <div class="main-txt">
        <h2>FACE</h2>
        <p>BLUSH</p>
        <p>CONCEALER</p>
        <p>CONTOUR & HIGHTLIGHT</p>
        <p>FOUNDATION</p>
        <p>POWDER</p>
        <p>PRIME & SET</p>
      </div>
      <div class="main-txt">
        <img src="@/assets/img/Navbar/Lipgloss.webp" />
        <h3>PRETTY & PLUMP LIPSTICK</h3>
        <img src="@/assets/img/Navbar/Break.jpg" />
        <h3>BREAK FREE EYESHADOW PALETTE</h3>
      </div>
      <div class="main-txt">
        <img src="@/assets/img/Navbar/KeepItPlay.webp" />
        <h3>KEEP IT PLAYFUL EYESHADOW PALETTE</h3>
        <img src="@/assets/img/Navbar/Makeup.jpg" />
        <h3>MAKE UP REMOVE WIPES</h3>
      </div>
      <div class="main-txt">
        <img src="@/assets/img/Navbar/Lipstick.webp" />
        <h3>LIP ATTRACTION LIPSTICK</h3>
        <img src="@/assets/img/Navbar/Pastel.jpg" />
        <h3>PASTEL GEL EXTEME SHINE POLISH</h3>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.main {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  max-width: 1200px;
  margin: auto;
}
.main-txt img {
  padding-top: 30px;
  max-width: 180px;
}

.main-txt h3 {
  text-align: center;
  font-size: 1rem;
  padding-top: 1rem;
}

h2 {
  font-size: 1rem;
  padding-top: 1rem;
  color: #e9008a;
}

p {
  font-size: 0.9rem;
  padding-top: 1rem;
}
</style>