<template>
  <div id="app">
    <keep-alive>
      <component :is="component"></component>
    </keep-alive>
    <button @click="component = 'FormOne'">render FormOne</button>
    <button @click="component = 'FormTwo'">render FormTwo</button>
  </div>
</template>

<script>
import FormOne from "./components/FormOne";
import FormTwo from "./components/FormTwo";
export default {
  name: "app",
  components: {
    FormOne,
    FormTwo
  },
  data() {
    return {
      component: "FormOne"
    };
  }
};
</script>

<style>
</style>
