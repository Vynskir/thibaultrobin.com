<template>
  <div id="app">
    <Header />
    <Home />
    <About />
    <Portfolio />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Home from "@/components/Home";
import About from "@/components/About";
import Portfolio from "@/components/Portfolio";
import Footer from "@/components/Footer";
import AOS from "aos";
import "aos/dist/aos.css";

AOS.init();

export default {
  name: "App",
  components: {
    Header,
    Home,
    About,
    Portfolio,
    Footer
  }
};
</script>

<style>
@import url("https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/css/bootstrap.min.css");
@import url("https://fonts.googleapis.com/css2?family=Secular+One&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Rubik:ital,wght@0,400;0,800;1,400;1,800&display=swap");
#app {
  margin: 88px 0 0;
  padding: 0;
  box-sizing: border-box;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  background: url(assets/images/bg.jpg) fixed center center no-repeat;
  -webkit-background-size: cover;
  -moz-background-size: cover;
  -o-background-size: cover;
  background-size: cover;
}
body {
  font-family: "Rubik", sans-serif;
}
h1,
h2,
h3,
h4,
h5,
h6 {
  color: #ffffff;
  text-shadow: 2px 2px 5px #000;
  font-weight: 800;
}

h1 {
  font-size: 5em;
}
h2 {
  font-size: 3em;
}
h3 {
  font-size: 2em;
}
.hx {
  font-size: 3.75em;
}

/* Tablet */
@media (min-width: 768px) and (max-width: 991px) {
  h1 {
    font-size: 4em;
  }
  h2 {
    font-size: 2.5em;
  }
  h3 {
    font-size: 1.5em;
  }
  .hx {
    font-size: 3em;
  }
}

/* Mobile */
@media (max-width: 767px) {
  h1 {
    font-size: 3em;
  }
  h2 {
    font-size: 2em;
  }
  h3 {
    font-size: 1em;
  }
  .hx {
    font-size: 2.2em;
  }
}

.section {
  padding-bottom: 8em;
}
.section-header {
  padding-top: 1em;
  padding-bottom: 1em;
  border-top: 5px solid #fff;
}
.section-header h1 {
  margin: 0;
}
.section-subtitle {
  padding-top: 1em;
  padding-bottom: 1.5em;
  font-style: italic;
  font-weight: 400;
}
.glass-blue {
  background-color: rgba(34, 23, 78, 0.2);
  backdrop-filter: blur(5px);
}
.glass-red {
  background-color: rgba(78, 49, 23, 0.2);
  backdrop-filter: blur(5px);
}
.typed-cursor {
  float: left;
}
</style>
