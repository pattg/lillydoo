<template>
  <section class="container-fluid bright">
    <div class="row">
      <div class="col-xs-12 text-center">
        <h2>Dein Testpaket enthält</h2>
      </div>
    </div>
    <div class="row">
      <div class="col-xs-12 col-sm-6">
        <div class="trial-image">
          <img src="../assets/img/lillydoo-little-blowballs-design-preview-tp.jpg">
        </div>
        <div class="trial-text">
          <ul>
            <h4>10 Lillidoo Windeln</h4>
            <li>0 % Parfüme & Lotionen, 100 % LILLYDOO Schutz</li>
            <li>Extra weich und mit idealer Passform</li>
          </ul>
        </div>
      </div>
      <div class="col-xs-12 col-sm-6">
        <div class="trial-image">
          <img src="../assets/img/water-wipes-15-small.jpg">
        </div>
        <div class="trial-text">
          <ul>
            <h4>15 Feuchttücher mit 99 % Wasser</h4>
            <li>0 % Parfüme & PEGs, 100 % biologisch abbaubar</li>
            <li>Natürlich rein, extra mild, Alternative zu "Wasser & Watte"</li>
          </ul>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "YourTrialPackage"
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

.trial-text li {
  list-style: none;
}
</style>


