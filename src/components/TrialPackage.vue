<template>
  <section id="trialPackage">
    <div class="row">
      <div class="small-12 medium-6 columns">
        <div class="oekotex-wrapper">
          <img src="../assets/img/oekotex_de.png" alt="oekotex-Logo" class="oekotex-logo">
          <img :src="products[selectedProduct].src" :alt="products[selectedProduct].name">
        </div>
      </div>
      <div class="small-12 medium-5 columns">
        <form>
          <h2>Unser gratis Testpaket</h2>
          <div class="btns-container">
            <p>Wähle Deine Größe</p>
            <ul class="btns">
              <li
                v-for="(product, index) in products"
                :key="index"
                :class="{active: selectedProduct == index }"
                @click="selectSet(index)"
                class="btn"
              >
                <p>{{index+1}}</p>
                <span>({{product.weight}})</span>
              </li>
            </ul>
          </div>
          <p>Teste jetzt unsere Windeln und Feuchttücher - In Größe 1 - 3 enthält unser Testpaket unsere Feuchttücher mit 99 % Wasser, ab Gr. 4 erhältst Du unsere Sensitiven Feuchttücher. Wir zahlen die Produkte, Du nur den Versand.</p>
          <ul class="product-info">
            <li
              class="primary-color"
            >Automatischer Übergang ins jederzeit kündbare Windel-Abo für 49,50 € pro Lieferung.</li>
            <li>
              Preise inkl. MwSt., ggf. zzgl.
              <a href="#">Versankosten</a>
            </li>
          </ul>
          <div class="trial-box-btn">
            <button class="btn-send" @click="addToCart">
              <span>IN DEN WARENKORB LEGEN</span>
            </button>
          </div>
        </form>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "TrialPackage",
  props: {
    products: {
      type: Array
    }
  },

  data() {
    return {
      selectedProduct: 0
    };
  },

  methods: {
    selectSet: function(index) {
      this.selectedProduct = index;
      this.$emit("selectSet", index);
    },
    addToCart: function() {
      alert("Habt einen schönen Tag ;)");
    }
  }
};
</script>

<style lang="scss" scoped>
@import "../scss/styles.scss";

.text-center img {
  width: 80%;
}

.trial-package-item {
  width: 100%;
  height: auto;
}

.btns-container {
  margin-bottom: 30px;
}

.btns li {
  text-align: center;
  width: 30%;
  padding: 7px 5px 2px 5px;
  margin-right: 10px;
}

.btns-container li:hover {
  background-color: #00afab;
  border-color: #00afab;
  color: #fff;
  cursor: pointer;
}

.btns-container li p {
  font-size: 1.3rem;
  line-height: 1;
  margin: 0;
}

.btns-container li span {
  line-height: 1;
  font-size: 0.8rem;
}

.btns {
  display: flex;
  list-style: none;
  justify-content: space-between;
  padding: 0;
  margin: 0;
}

.btns ul {
  padding: 0;
}

.btns li {
  text-align: center;
}

.btn {
  border: 1px solid #7c7c7c;
  width: 30%;
  padding: 7px 5px 2px 5px;
  margin-right: 10px;
}

.active {
  background-color: #00afab;
  border-color: #00afab;
  color: #fff;
}

.btn-send {
  border-radius: 0;
  border-style: solid;
  border-width: 0;
  cursor: pointer;
  font-family: Helvetica, Arial, sans-serif;
  font-weight: 400;
  line-height: normal;
  margin: 0 0 2rem;
  position: relative;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  padding: 0.5rem;
  font-size: 1.2rem;
  background-color: #00afab;
  border-color: #99dfdd;
  color: #fff;
  transition-property: background-color;
  transition-duration: 0.3s;
  transition-timing-function: ease-out;
  transition-delay: 0s;
  width: 100%;
}

.btn-send:hover {
  background-color: #99dfdd;
  color: white;
}

.product-info {
  padding: 0;
  margin-left: 1.1rem;
}

.oekotex-wrapper {
  position: relative;
}

.oekotex-logo {
  position: absolute;
}

.oekotex-wrapper .oekotex-logo {
  top: 10%;
  left: 9%;
  z-index: 10;
  width: 27%;
}

/*MEDIA QUERYS*/

@media only screen and (max-width: 834px) {
  .btns-container ul {
    justify-content: initial;
    flex-direction: row;
    flex-wrap: wrap;
    height: 140px;
  }
}

@media only screen and (max-width: 834px) {
  .btns-container ul li {
    margin-bottom: 10px;
  }
}

@media only screen and (max-width: 834px) {
  .small-12 {
    width: 100%;
    height: 100%;
  }
}
</style>
