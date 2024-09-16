<template>
  <div>
    <link href="https://unpkg.com/@blueprintjs/core@5/lib/css/blueprint.css" rel="stylesheet" />
    <div id="app"></div>
  </div>
</template>

<script>
import { createDemoApp } from "polotno/polotno-app";

export default {
  name: "App",
  mounted() {
    const { store } = createDemoApp({
      container: document.getElementById("app"),
      key: "6633iO-JQydxYQgUQhYr", // you can create it here: https://polotno.com/cabinet/
      // you can hide back-link on a paid license
      // but it will be good if you can keep it for Polotno project support
      showCredit: true,
    });
  },
};
</script>

<style global>
#app {
  width: 100vw;
  height: 100vh;
}

body {
  padding: 0;
  margin: 0;
}
</style>