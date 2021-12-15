<template>
  <div id="app">
    <Navigation />
    <router-view />
  </div>
</template>

<script>
import Navigation from "./components/Navigation.vue";
export default {
  components: {
    Navigation,
  },
};
</script>


<style>
@import url("https://fonts.googleapis.com/css2?family=Open+Sans:wght@300;400;600&family=Outfit:wght@300;400;600&display=swap");
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body,
input,
textarea,
button {
  font-family: "Open Sans", sans-serif;
}

:root {
  --clr-bg: #ededed;
  --clr-border: #d2d2d2;
}

button {
  width: 40px;
  height: 40px;
  border-radius: 50px;
  background-color: var(--clr-bg);
  border: 1px solid var(--clr-border);
  box-shadow: 0 0px 5px 0 rgba(0, 0, 0, 0.2);
}

button:hover {
  cursor: pointer;
}
</style>
