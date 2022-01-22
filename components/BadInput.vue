
<template>
  <div class="my-input">
    <label>{{label}}</label>
    <input
      :placeholder="inputPlaceholder"
      @input="handleInput"
    >
    <button @click="handleClick">Click</button>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    label: String,
    inputPlaceholder: String,
  },
  methods: {
    handleInput(newVal) {
      this.$emit('input', newVal);
    },
    handleClick() {
      this.$emit('confirm');
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.my-input {
  display: flex;
  flex-flow: column;
}
.my-input label {
  color: grey;
  font-family: helvetica;
}
.my-input input {
  margin-top: 7px;
  border: 1px solid #efefef;
  height: 35px;
  border-radius: 5px;
  padding: 0 5px;
}
.my-input input::placeholder {
  color: #aaaaaa;
}
.my-input button {
  margin-top: 4px;
  height: 30px;
  border: none;
  background: #3475ab;
  border-radius: 5px;
  color: white;
}
</style>
