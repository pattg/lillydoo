<template>
  <section class="container-fluid dark">
    <div class="row">
      <div class="col-xs-12 text-center">
        <h2>Wie es funktioniert</h2>
      </div>
    </div>
    <div class="row">
      <div class="col-xs-12 col-sm-4 text-center">
        <img src="../assets/img/lillydoo-your-trialbox-icon.svg">
        <h4>Dein Testpaket</h4>
        <p>
          Wir schenken Dir die Produkte,
          <br>Du übernimmst nur das Porto.
        </p>
      </div>
      <div class="col-xs-12 col-sm-4 text-center">
        <img src="../assets/img/lillydoo-your-flexibility-icon.svg">
        <h4>Deine Flexibilität</h4>
        <p>
          Erste Monatsbox nach 14 Tagen für 49,50€ erhalten.
          <br>Oder noch vor der ersten Lieferung kündigen.
        </p>
        <p>
          <a href="####">Erfahre hier mehr über das LILLYDOO Windel-Abo</a>
        </p>
      </div>
      <div class="col-xs-12 col-sm-4 text-center">
        <img src="../assets/img/lillydoo-your-subscription-icon.svg">
        <h4>Deine Monatsbox</h4>
        <p>
          Jederzeit Designs oder Lieferintervalle anpassen oder
          <br>die Windelgröße ändern
        </p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "HowItWorks"
};
</script>

<style lang="scss" scoped>
section.dark {
  background: #f8f8f8;
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
</style>
