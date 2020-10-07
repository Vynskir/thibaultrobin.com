<template>
  <div id="about" class="section glass-red">
    <div class="section-header">
      <h2>ABOUT ME</h2>
    </div>
    <div class="container">
      <h3 class="section-subtitle">
        5+ years of experience in the development of tools and workflows
      </h3>
      <div data-aos="fade-right" class="logos row">
        <img src="@/assets/logos/java.png" alt="Java" />
        <img src="@/assets/logos/python.png" alt="Python" />
        <img src="@/assets/logos/r.png" alt="R" />
        <img src="@/assets/logos/javascript.png" alt="JavaScript" />
        <img src="@/assets/logos/d3.png" alt="D3.js" />
        <img src="@/assets/logos/bootstrap.png" alt="Bootstrap" />
        <img src="@/assets/logos/docker.png" alt="Docker" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "About"
};
</script>

<style scoped>
.logos {
  justify-content: center;
}
.logos img {
  width: 6em;
  height: 6em;
  margin: 1em;
  border-radius: 1.3em;
  background-color: #fff;
  box-shadow: 0 0.15rem 0.25rem rgba(0, 0, 0, 0.8);
}
</style>
