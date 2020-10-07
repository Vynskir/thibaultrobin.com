<template>
  <nav class="navbar fixed-top navbar-expand-sm navbar-dark shadow">
    <span class="navbar-brand">Thibault Robin</span>
    <button
      class="navbar-toggler"
      type="button"
      data-toggle="collapse"
      data-target="#navbarNav"
      aria-controls="navbarNav"
      aria-expanded="false"
      aria-label="Toggle navigation"
    >
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNav">
      <ul class="navbar-nav">
        <li class="nav-item">
          <a class="nav-link" href="#home" @click="scrollIntoView">Home</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#about" @click="scrollIntoView">About</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#portfolio" @click="scrollIntoView"
            >Portfolio</a
          >
        </li>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {
  name: "Header",
  methods: {
    scrollIntoView(evt) {
      evt.preventDefault();

      const href = evt.target.getAttribute("href");
      const el = href ? document.querySelector(href) : null;

      if (el) {
        const pos = document.querySelector(href).offsetTop - 88;
        window.scroll({ top: pos, behavior: "smooth" });
      }
    }
  }
};
</script>

<style scoped>
@font-face {
  font-family: mystique;
  src: url(../assets/fonts/Mystique.ttf);
}
nav {
  min-height: 88px;
  background-color: #131313;
}
.navbar-brand {
  padding: 0;
  font-size: 3em;
  font-family: mystique, sans-serif;
}
a.nav-link {
  font-size: 1.25em;
  font-family: "Secular One", sans-serif;
}
a {
  color: rgba(255, 255, 255, 0.5);
}
a:hover {
  text-decoration: none;
  cursor: pointer;
  color: rgba(255, 255, 255, 0.8);
}
a.active {
  color: rgba(255, 255, 255, 1);
}
</style>
