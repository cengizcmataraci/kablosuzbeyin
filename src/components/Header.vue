<template>
  <div class="app">
    <nav
      class="navbar navbar-expand-lg navbar-dark container-fluid fixed-top"
      :class="{ 'navbar--hidden': !showNavbar }"
      style="height: 2.2em; background-color: #bf1e2d;"
      id="navbar"
    >
      <div class="container-fluid justify-content-start">
        <a href="#"><img src="../assets/logo.png" alt=""/></a>
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarText"
          aria-controls="navbarText"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
      </div>

      <ul class="nav container-fluid justify-content-end" style="color: white;">
        <li class="nav-item ">
          <a
            class="nav-link active text-light"
            aria-current="page"
            href="#hakkimizda"
            >Hakkımızda</a
          >
        </li>
        <li class="nav-item">
          <a class="nav-link text-light" href="#etkinlikler">Etkinliklerimiz</a>
        </li>
        <li class="nav-item">
          <a class="nav-link text-light" href="#anlasmalar">Anlaşmalarımız</a>
        </li>
        <li class="nav-item">
          <a class="nav-link text-light" href="#iletisim">İletişim</a>
        </li>
      </ul>
    </nav>
  </div>
</template>

<script>
export default {
  data() {
    return {
      showNavbar: true,
      lastScrollPosition: 0,
    };
  },
  mounted() {
    window.addEventListener("scroll", this.onScroll);
  },
  beforeDestroy() {
    window.removeEventListener("scroll", this.onScroll);
  },
  methods: {
    onScroll() {
      const currentScrollPosition =
        window.pageYOffset || document.documentElement.scrollTop;

      if (currentScrollPosition < 0) {
        return;
      }

      this.showNavbar = currentScrollPosition < this.lastScrollPosition;

      this.lastScrollPosition = currentScrollPosition;
    },
  },
};
</script>

<style scoped>
* {
  box-sizing: border-box;
}
body {
  padding: 0;
  margin: 0;
}
.app {
  width: 100vw;
}
.navbar {
  height: 60px;
  width: 100vw;
  position: fixed;
  box-shadow: 0 2px 15px rgba(71, 120, 120, 0.5);
  transform: translate3d(0, 0, 0);
  transition: 0.1s all ease-out;
}
.navbar.navbar--hidden {
  box-shadow: none;
  transform: translate3d(0, -100%, 0);
}
</style>
