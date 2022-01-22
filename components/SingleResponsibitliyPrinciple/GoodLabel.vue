
<template>
  <div class="good-label">
    <label :style="{ color }">{{text}}</label>
  </div>
</template>

<script>
export default {
  name: "GoodLabel",
  props: {
    text: String,
    color: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.good-label {
  display: flex;
  flex-flow: column;
}
.good-label label {
  font-family: helvetica;
  font-size: 14px;
}
</style>
