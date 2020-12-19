<template>
  <div id="App">
    <Header />
    <Welcome />
    <about-content />
    <Slider />
    <Support />
    <Contact />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header";
import Footer from "./components/Footer";
import Slider from "./components/Slider";
import aboutContent from "./components/aboutContent";
import Welcome from "./components/Welcome";
import Support from "./components/Support";
import Contact from "./components/Contact";



export default {
  name: "App",
  components: {
    Header,
    Footer,
    Slider,
    aboutContent,
    Welcome,
    Support,
    Contact,
  },
};
</script>

<style>
body {
  margin: 0px;
}
</style>
