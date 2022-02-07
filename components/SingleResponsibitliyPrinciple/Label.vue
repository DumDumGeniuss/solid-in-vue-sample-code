
<template>
  <div class="component-root">
    <label :style="{ color }">{{text}}</label>
  </div>
</template>

<script>
export default {
  name: "Label",
  props: {
    text: String,
    color: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.component-root {
  display: flex;
  flex-flow: column;
}
.component-root label {
  font-family: helvetica;
  font-size: 14px;
}
</style>
