<template>
  <div>
    <!-- <slot name="title"></slot>
    <hr />
    <h1>i am the form helper</h1>
    <hr />
    <slot name="text"></slot>-->
    <h1>slot插槽，可作为占位使用，通过父级组件传递需要展示</h1>
    <form action>
      <div id="form-header">
        <slot name="form-header"></slot>
      </div>
      <div id="form-fields">
        <slot name="form-fields"></slot>
      </div>
      <div id="form-controls">
        <slot name="form-controls"></slot>
      </div>
      <div id="userful-links">
        <ul>
          <li>
            <a href="#">LINK1</a>
          </li>
          <li>
            <a href="#">LINK2</a>
          </li>
          <li>
            <a href="#">LINK3</a>
          </li>
          <li>
            <a href="#">LINK4</a>
          </li>
        </ul>
      </div>
    </form>
  </div>
</template>

<script>
export default {
  name: "FormHelper"
};
</script>

<style scoped>
</style>
