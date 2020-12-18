<template>
  <div id="App">
    <Header />
    <Welcome />
    <about-content />
    <Slider />
    <br />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header";
import Footer from "./components/Footer";
import Slider from "./components/Slider";
import aboutContent from "./components/aboutContent";
import Welcome from "./components/Welcome";


export default {
  name: "App",
  components: {
    Header,
    Footer,
    Slider,
    aboutContent,
    Welcome,

  },
};
</script>

<style>
body {
  margin: 0px;
}
</style>
