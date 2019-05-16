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
        <div class="small-8 trial-info">
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
            :alt="products[selectedProduct].name"
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
section.bright {
  background: #fff;
  flex-direction: column;
}

.text-center {
  text-align: center !important;
}

.row {
  margin: 0 auto;
  max-width: 80rem;
  width: 100%;
  padding: 2rem 0 2rem 0;
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

.trial-image {
  float: left;
}
.trial-text {
  float: left;
}

.ul {
  margin-left: 1.1rem;
}
</style>


