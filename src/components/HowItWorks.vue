<template>
  <section class="dark">
    <div class="row dark">
      <div class="small-12 columns text-center">
        <h2>Wie es funktioniert</h2>
      </div>
    </div>
    <div class="row">
      <div class="small-12 medium-4 columns text-center">
        <img src="../assets/img/lillydoo-your-trialbox-icon.svg">
        <h4>Dein Testpaket</h4>
        <p>
          Wir schenken Dir die Produkte,
          <br>Du übernimmst nur das Porto.
        </p>
      </div>
      <div class="small-12 medium-4 columns text-center">
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
      <div class="small-12 medium-4 columns text-center">
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
@import "../scss/styles.scss";

.row {
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
/*MEDIA QUERYS*/

@media only screen and (max-width: 834px) {
  .small-12 {
    width: 100%;
  }
}
</style>
