<template>
  <section>
    <div class="hero-header mobile-full-vh">
      <img src="../assets/img/oekotex_de.png" class="oekotex-logo">
      <div class="row text-center">
        <div class="small-12 medium-6 end columns">
          <h1>Entdecke unsere Hautfreundlichkeit</h1>
          <div class="button-wrapper">
            <a href="#trialPackage" class="button">Jetzt Deine Größe wählen</a>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "HeroHeader"
};
</script>

<style lang="scss" scoped>
@import "../scss/styles.scss";
.hero-header {
  background: (url("../assets/img/lillydoo-testpaket-header-large.jpg"))
    no-repeat center center/cover;
  width: 100%;
  height: 37vw;
  min-height: 320px;
  max-height: 500px;
  display: flex;
  align-items: center;
  position: relative;
}

.row {
  max-width: 80rem;
  width: 100%;
}
.oekotex-logo {
  position: absolute;
  top: 14%;
  right: 3%;
  width: 12%;
}

h1 {
  font-family: Helvetica, sans-serif;
  font-size: 2.625rem;
  font-weight: normal;
  line-height: 1.1;
  margin-bottom: 20px;
}
.button {
  margin-top: 30px;
  margin-bottom: 10px;
  font-size: 0.2rem;
  padding: 0 10px;
  min-width: 13rem;
  line-height: 2.8;
}

.button,
button {
  -webkit-appearance: none;
  -moz-appearance: none;
  border-radius: 0;
  border-style: solid;
  border-width: 0;
  cursor: pointer;
  font-family: Helvetica, Arial, sans-serif;
  font-size: 1.2rem;
  line-height: normal;
  margin: 0 0 1rem;
  position: relative;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  padding: 1.2rem 2.5rem 1.2rem 2.5rem;
  font-size: 1rem;
  background-color: #00afab;
  border-color: #99dfdd;
  color: #fff;
  transition: 0.3s;
  text-transform: uppercase;
}

.button:hover {
  background-color: #99dfdd;
  color: white;
}

.oekotex-logo {
  position: absolute;
  top: 56%;
  right: 0%;
  width: 25%;
}

/*MEDIA QUERYS*/

@media only screen and (max-width: 834px) {
  .hero-header {
    background: (url("../assets/img/lillydoo-testpaket-header-medium.jpg"))
      no-repeat center center/cover;
    display: block;
    width: auto;
    height: 81vw;
    max-height: 550px;
  }
}

@media only screen and (max-width: 414px) {
  .hero-header {
    background: (url("../assets/img/lillydoo-testpaket-header-small.jpg"))
      no-repeat center center/cover;
    display: block;
    width: auto;
    height: 100vh;
  }
}

@media only screen and (max-width: 834px) {
  .hero-header .mobile-full-vh {
    height: 100vh;
  }
}

@media (min-width: 600px) {
  .hero-header .oekotex-logo {
    top: 49%;
    right: 12%;
    width: 18%;
  }
}

@media (max-width: 600px) {
  .hero-header .button {
    width: 80%;
  }
}

@media (min-width: 900px) {
  .hero-header .oekotex-logo {
    top: 14%;
    right: 3%;
    width: 12%;
  }
}

@media only screen and (max-width: 834px) {
  .hero-header .row {
    height: 70%;
  }
}

@media only screen and (max-width: 834px) {
  .hero-header .row > .columns {
    display: flex;
    -webkit-flex-direction: column;
    -ms-flex-direction: column;
    flex-direction: column;
    -webkit-flex-wrap: nowrap;
    -ms-flex-wrap: nowrap;
    flex-wrap: nowrap;
    -webkit-justify-content: center;
    -ms-flex-pack: center;
    justify-content: center;
    height: 100%;
  }
}
@media only screen and (max-width: 834px) {
  .small-12 {
    width: 100%;
  }
}
</style>
