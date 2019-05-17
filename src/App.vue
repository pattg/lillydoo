<template>
  <div>
    <HeroHeader></HeroHeader>
    <TrialPackage :products="products" @selectSet="onSelectSet"></TrialPackage>
    <HowItWorks></HowItWorks>
    <YourTrialPackage :products="products" :selectedProduct="index"></YourTrialPackage>
  </div>
</template>

<script>
import HeroHeader from "./components/HeroHeader";
import TrialPackage from "./components/TrialPackage";
import HowItWorks from "./components/HowItWorks";
import YourTrialPackage from "./components/YourTrialPackage";
export default {
  name: "App",
  data() {
    return {
      products: [
        {
          name: "lillydoo-testpaket-10",
          src: require("./assets/img/lillydoo-testpaket-10.jpg"),
          weight: "2-3 KG",
          headline: "15 Feuchtücher mit 99% Wasser",
          bp1: "0% Parfüme & PEGs, 100% biologisch abbaubar",
          bp2: "Natürlich rein, extra mild, Alternative zu Wasser und Watte",
          yourTrialPackageSrc: require("./assets/img/water-wipes-15-small.jpg"),
          yourTrialPackageAltName: "15 Feuchtücher mit 99% Wasser"
        },

        {
          name: "lillydoo-testpaket-20",
          src: require("./assets/img/lillydoo-testpaket-20.jpg"),
          weight: "3-4 KG",
          headline: "15 Feuchtücher mit 99% Wasser",
          bp1: "0% Parfüme & PEGs, 100% biologisch abbaubar",
          p2: "Natürlich rein, extra mild, Alternative zu Wasser und Watte",
          yourTrialPackageSrc: require("./assets/img/water-wipes-15-small.jpg"),
          yourTrialPackageAltName: "15 Feuchtücher mit 99% Wasser"
        },

        {
          name: "lillydoo-testpaket-30",
          src: require("./assets/img/lillydoo-testpaket-30.jpg"),
          weight: "4-7 KG",
          headline: "15 Feuchtücher mit 99% Wasser",
          bp1: "0% Parfüme & PEGs, 100% biologisch abbaubar",
          bp2: "Natürlich rein, extra mild, Alternative zu Wasser und Watte",
          yourTrialPackageSrc: require("./assets/img/water-wipes-15-small.jpg"),
          yourTrialPackageAltName: "15 Feuchtücher mit 99% Wasser"
        },
        {
          name: "lillydoo-testpaket-40",
          src: require("./assets/img/lillydoo-testpaket-40.jpg"),
          weight: "7-10 KG",
          headline: "15 sensitive Feuchttücher",
          bp1: "0% Parfüme & PEGs, 100% biologisch abbaubar",
          bp2: "Extra dickes und komposierbares Tuch",
          yourTrialPackageSrc: require("./assets/img/sensitive-wipes-15-small.jpg"),
          yourTrialPackageAltName: "15 sensitive Feuchttücher"
        },

        {
          name: "lillydoo-testpaket-50",
          src: require("./assets/img/lillydoo-testpaket-50.jpg"),
          weight: "10-12 KG",
          headline: "15 sensitive Feuchttücher",
          bp1: "0% Parfüme & PEGs, 100% biologisch abbaubar",
          bp2: "Extra dickes und komposierbares Tuch",
          yourTrialPackageSrc: require("./assets/img/sensitive-wipes-15-small.jpg"),
          yourTrialPackageAltName: "15 sensitive Feuchttücher"
        }
      ],
      index: 0
    };
  },
  components: {
    HeroHeader,
    TrialPackage,
    HowItWorks,
    YourTrialPackage
  },
  methods: {
    onSelectSet(index) {
      this.index = index;
    }
  }
};
</script>

<style lang="scss">
@import "~foundation-sites/scss/foundation.scss";
@include foundation-everything;
</style>
