
<template>
  <div class="good-input">
    <input
      :placeholder="placeholder"
      @input="handleInput"
    >
  </div>
</template>

<script>
export default {
  name: "GoodInput",
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
.good-input {
  display: flex;
}
.good-input input {
  width: 100%;
  border: 1px solid #cfcfcf;
  height: 35px;
  border-radius: 5px;
  padding: 0 5px;
}
.good-input input::placeholder {
  color: #aaaaaa;
}
</style>
