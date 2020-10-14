<template>
  <div>
    <Header />
  </div>
</template>

<script>
import Header from "./components/Layout/Header";

export default {
  name: "App",
  components: {
    Header,
  },
};
</script>

<style>
body {
  margin: 0;
  padding: 0;
}

a {
  font-family: Lato;
}
</style>
