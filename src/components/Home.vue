<template>
  <div id="home">
    <div data-aos="zoom-in" data-aos-duration="1500">
      <h1 class="text-shadow">Hi, I'm Thibault Robin</h1>
      <div class="typed-container hx">
        <div class="typed text-shadow"></div>
      </div>
    </div>
  </div>
</template>

<script>
import Typed from "typed.js";

export default {
  name: "Home",
  mounted() {
    new Typed(".typed", {
      strings: [
        "PhD in Bioinformatics. ",
        "Full Stack Developer. ",
        "Data Analyst. "
      ],
      typeSpeed: 60,
      backDelay: 1000,
      loop: true
    });
  }
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Cousine&display=swap");

#home {
  display: flex;
  justify-content: center;
  flex-direction: column;
  height: calc(100vh - 88px);
  width: 100%;
  color: #ffffff;
}
.typed-container {
  display: flex;
  justify-content: center;
  font-family: "Cousine", monospace;
  color: #ffffff;
  text-shadow: 2px 2px 5px #000;
}
</style>
