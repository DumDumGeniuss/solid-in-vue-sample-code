
<template>
  <div class="component-root">
    <input
      :placeholder="placeholder"
      @input="handleInput"
    >
  </div>
</template>

<script>
export default {
  name: "Input",
  props: {
    placeholder: String,
  },
  methods: {
    handleInput(newVal) {
      this.$emit('textChange', newVal);
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.component-root {
  display: flex;
}
.component-root input {
  width: 100%;
  border: 1px solid #cfcfcf;
  height: 35px;
  border-radius: 5px;
  padding: 0 5px;
}
.component-root input::placeholder {
  color: #aaaaaa;
}
</style>
