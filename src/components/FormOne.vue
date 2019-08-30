<template>
  <div class="hello">
    <FormHelper>
      <!-- <h2 slot="title">{{title}}</h2>
      <p slot="text">Lorem ipsum dolor sit amet.</p>-->
      <div slot="form-header">
        <h3>FormOne</h3>
        <p>Lorem ipsum dolor sit amet.</p>
      </div>
      <div slot="form-fields">
        <input type="text" placeholder="name" />
        <input type="password" placeholder="password" />
      </div>
      <div slot="form-controls">
        <button @click="handleSubmit">Submit</button>
      </div>
    </FormHelper>
  </div>
</template>

<script>
import FormHelper from "./FormHelper";
export default {
  name: "FormOne",
  components: {
    FormHelper
  },
  methods: {
    handleSubmit() {
      alert("thanks for submitting");
    }
  }
};
</script>

<style scoped>
</style>
