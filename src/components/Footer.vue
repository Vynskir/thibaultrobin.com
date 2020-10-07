<template>
  <div>
    <a
      id="scroll-home"
      class="fas fa-angle-double-up"
      href="#"
      title="Go to the Top"
    ></a>
    <footer class="footer">
      <div class="links">
        <a
          class="fab fa-github-square"
          href="https://github.com/Vynskir/"
          title="Github"
          target="_blank"
        ></a>
        <a
          class="fab fa-linkedin"
          href="https://www.linkedin.com/in/thibault-robin/"
          title="LinkedIn"
          target="_blank"
        ></a>
        <a
          class="fas fa-envelope-square"
          href="mailto:robin.thibault@protonmail.com"
          title="Email"
        ></a>
      </div>
      <div class="copyright">
        © 2020 Thibault Robin
      </div>
    </footer>
  </div>
</template>
<script>
export default {
  name: "Footer"
};
</script>

<style scoped>
footer {
  padding-top: 1rem;
  padding-bottom: 1rem;
  color: rgba(255, 255, 255, 0.5);
  background-color: #333;
}
#scroll-home {
  position: absolute;
  font-size: 2.5em;
  background-color: #333;
  width: 1.5em;
  height: 1.5em;
  border-radius: 50%;
  padding-top: 0.25em;
  margin-top: -0.65em;
  margin-left: -0.75em;
}
.links {
  padding-top: 1.5em;
  padding-bottom: 0.5em;
}
.copyright {
  padding-top: 1em;
  padding-bottom: 1em;
  font-family: "Secular One", sans-serif;
}
.fab,
.fas {
  font-size: 2.5em;
  margin: 0.1em;
  color: rgba(255, 255, 255, 0.5);
}
.fab:hover,
.fas:hover {
  text-decoration: none;
  cursor: pointer;
  color: rgba(255, 255, 255, 0.8);
}
</style>
