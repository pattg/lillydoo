<template>
  <section>
    <div class="row">
      <div class="medium-12 text-center columns margin-top-20">
        <h2>Dein Testpaket enthält</h2>
      </div>
    </div>
    <div class="row">
      <div class="small-12 medium-6 margin-bottom-20 columns">
        <div class="trial-image small-3 trial-contains-img text-center">
          <img src="../assets/img/lillydoo-little-blowballs-design-preview-tp.jpg">
        </div>
        <div class="small-8 trial-text">
          <ul>
            <h4>10 Lillydoo Windeln</h4>
            <li>0 % Parfüme & Lotionen, 100 % LILLYDOO Schutz</li>
            <li>Extra weich und mit idealer Passform</li>
          </ul>
        </div>
      </div>
      <div class="small-12 medium-6 margin-bottom-20 columns">
        <div class="trial-image small-3 text-center">
          <img
            :src="products[selectedProduct].yourTrialPackageSrc"
            :alt="products[selectedProduct].yourTrialPackageAltName"
          >
        </div>
        <div class="trial-text small-8">
          <ul>
            <h4>{{products[selectedProduct].headline}}</h4>
            <li>{{products[selectedProduct].bp1}}</li>
            <li>{{products[selectedProduct].bp2}}</li>
          </ul>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "YourTrialPackage",
  props: {
    products: {
      type: Array
    },
    selectedProduct: Number
  }
};
</script>

<style lang="scss" scoped>
@import "../scss/styles.scss";

.row {
  max-width: 80rem;
}

p {
  display: block;
}

h2 {
  font-family: Helvetica, sans-serif;
  font-size: 1.625rem;
  font-weight: normal;
  line-height: 1.1;
  margin-bottom: 10px;
}

h4 {
  text-transform: uppercase;
  font-size: 1.1rem;
  font-weight: 500;
}

.trial-image {
  float: left;
}
.trial-text {
  float: left;
}

.ul {
  margin-left: 1.1rem;
  padding-left: 0;
}

ul li {
  list-style-position: inside;
}

/*MEDIA QUERYS*/

@media only screen and (max-width: 834px) {
  .small-12 {
    width: 100%;
  }
}
</style>


