<template>
  <main-screen v-if="statusMatch === 'default'" @onStart="onHandleBeforeStart()"/>
  <interactive-screen v-if="statusMatch === 'match'"/>
  <copy-right/>
</template>

<script>
import MainScreen from "./components/MainScreen.vue";
import CopyRight from "./components/CopyRight.vue";
import InteractiveScreen from "./components/InteractiveScreen.vue";
// import ResultScreen from "./components/ResultScreen.vue";

export default {
  name: "App",
  data(){
    return {
      statusMatch: "default",
    }
  },
  components: { MainScreen,CopyRight,InteractiveScreen },
  methods: {
    onHandleBeforeStart() {
      this.statusMatch = "match";
    }
  }
};
</script>

<style></style>
