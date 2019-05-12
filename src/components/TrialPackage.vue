<template>
  <section class="container-fluid">
    <div class="row">
      <div class="col-sm-6 text-center">
        <img src="../assets/img/lillydoo-testpaket-10.jpg">
      </div>
      <div class="col-sm-6">
        <form>
          <h2>Unser gratis Testpaket</h2>
          <div class="btns-container">
            <p>Wähle Deine Größe</p>
            <ul class="btns">
              <li class="btn" @click="activeBtn = 'btn1'" :class="{active : activeBtn == 'btn1'}">
                <p>1</p>
                <span>(2-3 KG)</span>
              </li>
              <li class="btn" @click="activeBtn = 'btn2'" :class="{active : activeBtn == 'btn2'}">
                <p>2</p>
                <span>(3-4 KG)</span>
              </li>
              <li class="btn" @click="activeBtn = 'btn3'" :class="{active : activeBtn == 'btn3'}">
                <p>3</p>
                <span>(4-7 KG)</span>
              </li>
              <li class="btn" @click="activeBtn = 'btn4'" :class="{active : activeBtn == 'btn4'}">
                <p>4</p>
                <span>(7-10 KG)</span>
              </li>
              <li class="btn" @click="activeBtn = 'btn5'" :class="{active : activeBtn == 'btn5'}">
                <p>5</p>
                <span>(10-12 KG)</span>
              </li>
            </ul>
          </div>
          <p>Teste jetzt unsere Windeln und Feuchttücher - In Größe 1 - 3 enthält unser Testpaket unsere Feuchttücher mit 99 % Wasser, ab Gr. 4 erhältst Du unsere Sensitiven Feuchttücher. Wir zahlen die Produkte, Du nur den Versand.</p>
          <ul class="product-info">
            <li>Automatischer Übergang ins jederzeit kündbare Windel-Abo für 49,50 € pro Lieferung.</li>
            <li>
              Preise inkl. MwSt., ggf. zzgl.
              <a href="#">Versankosten</a>
            </li>
          </ul>
          <div class="trial-box-btn">
            <button class="btn-send">
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
  data() {
    return { activeBtn: "btn1" };
  }
};
</script>

<style lang="scss" scoped>
.row {
  margin: 0 auto;
  max-width: 80rem;
  width: 100%;
  padding: 2rem 0 2rem 0;
}

.text-center {
  text-align: center !important;
}

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
  padding: 1.6rem 3.2rem 1.7rem 3.2rem;
  font-size: 1.6rem;
  background-color: #00afab;
  border-color: #99dfdd;
  color: #fff;
  transition-property: background-color;
  transition-duration: 0.3s;
  transition-timing-function: ease-out;
  transition-delay: 0s;
}

.btn-send:hover {
  background-color: #99dfdd;
  color: white;
}

.product-info {
  padding: 0;
  margin-left: 1.1rem;
}
</style>
