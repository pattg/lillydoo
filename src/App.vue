<template>
  <div>
    <HeroHeader></HeroHeader>
    <TrialPackage v-on:buttonClick="onButtonClick"></TrialPackage>
    <HowItWorks></HowItWorks>
    <YourTrialPackage></YourTrialPackage>
  </div>
</template>

<script>
import HeroHeader from "./components/HeroHeader";
import TrialPackage from "./components/TrialPackage";
import HowItWorks from "./components/HowItWorks";
import YourTrialPackage from "./components/YourTrialPackage";
export default {
  name: "App",
  components: {
    HeroHeader,
    TrialPackage,
    HowItWorks,
    YourTrialPackage
  },
  methods: {
    onButtonClick: buttonValue => {
      console.log(buttonValue);
    }
  }
};
</script>

<style lang="scss" scoped>
div {
  @import "./scss/styles.scss";
}
</style>
