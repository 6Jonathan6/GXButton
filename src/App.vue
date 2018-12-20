<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <gx-button class="button" @click="onClick('gx-button')">Soy un boton</gx-button>
    <yellow-button class="button" @click="onClick('yellow-button')">Soy un boton amarillo</yellow-button>
  </div>
</template>

<script>
import GxButton from "./components/GxButton.vue";
import YellowButton from "./components/YellowButton.vue";

export default {
  name: "app",
  methods: {
    onClick(message) {
      console.log(message);
    }
  },
  components: {
    GxButton,
    YellowButton
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.button {
  background: blue;
  border-radius: 5px;
}
.yellow {
  background: yellow;
  border-radius: 25%;
  height: 70px;
  width: 150px;
  color: white;
}
</style>
