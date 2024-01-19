<template>
  <MainScreen/>
  <CopyRight/>
</template>

<script>
import MainScreen from "./components/MainScreen.vue";
import CopyRight from "./components/CopyRight.vue";
// import InteractiveScreen from "./components/InteractiveScreen.vue";
// import ResultScreen from "./components/ResultScreen.vue";

export default {
  name: "App",
  components: { MainScreen,CopyRight },
};
</script>

<style></style>
