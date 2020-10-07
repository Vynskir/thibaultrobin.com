<template>
  <div id="portfolio" class="section glass-blue">
    <div class="section-header">
      <h2>PORTFOLIO</h2>
    </div>
    <div class="container">
      <h3 class="section-subtitle">Academic works</h3>
      <div class="card-deck">
        <div data-aos="flip-right" data-aos-delay="50" class="card mx-auto">
          <img
            class="card-img-top"
            src="@/assets/images/clastr.png"
            alt="Card image cap"
          />
          <div class="card-body">
            <div class="card-title">CLASTR</div>
            <p class="card-text">
              Search for similarities between cell line samples and the human
              cell line STR profiles stored in the Cellosaurus
            </p>
            <a
              href="https://web.expasy.org/cellosaurus-str-search/"
              class="btn btn-light"
              >Visit Website</a
            >
          </div>
        </div>
        <div data-aos="flip-right" data-aos-delay="100" class="card mx-auto">
          <img
            class="card-img-top"
            src="@/assets/images/compozitor.png"
            alt="Card image cap"
          />
          <div class="card-body">
            <div class="card-title">Compozitor</div>
            <p class="card-text">
              Display the glycan compositions stored in the GlyConnect database
              in the form of directed graphs
            </p>
            <a
              href="https://glyconnect.expasy.org/compozitor/"
              class="btn btn-light"
              >Visit Website</a
            >
          </div>
        </div>
        <div data-aos="flip-right" data-aos-delay="150" class="card mx-auto">
          <img
            class="card-img-top"
            src="@/assets/images/octopus.png"
            alt="Card image cap"
          />
          <div class="card-body">
            <div class="card-title">Octopus</div>
            <p class="card-text">
              Display the relationships between the glycan structures stored in
              the GlyConnect database
            </p>
            <a
              href="https://glyconnect.expasy.org/octopus/"
              class="btn btn-light"
              >Visit Website</a
            >
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Portfolio"
};
</script>

<style scoped>
.card {
  border-radius: 0.75em;
  overflow: hidden;
  min-width: 20em;
  max-width: 20em;
  box-shadow: 0px 0px 26px -3px rgba(0, 0, 0, 0.5);
}
.card-title {
  color: #333;
  font-size: 1.2em;
  font-weight: 800;
}
.btn {
  border: 1px solid rgba(0, 0, 0, 0.1);
}
</style>
