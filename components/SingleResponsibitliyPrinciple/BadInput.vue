
<template>
  <div class="bad-input">
    <label :style="{ color: labelColor }">{{label}}</label>
    <input
      :placeholder="inputPlaceholder"
      @input="handleInput"
    >
    <button @click="handleClick">{{buttonText}}</button>
  </div>
</template>

<script>
export default {
  name: "BadInput",
  props: {
    label: String,
    labelColor: String,
    inputPlaceholder: String,
    buttonText: String,
  },
  methods: {
    handleInput(newVal) {
      this.$emit('textChange', newVal);
    },
    handleClick() {
      this.$emit('buttonClick');
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.bad-input {
  display: flex;
  flex-flow: column;
}
.bad-input label {
  font-family: helvetica;
  font-size: 14px;
}
.bad-input input {
  margin-top: 7px;
  border: 1px solid #cfcfcf;
  height: 35px;
  border-radius: 5px;
  padding: 0 5px;
}
.bad-input input::placeholder {
  color: #aaaaaa;
}
.bad-input button {
  margin-top: 4px;
  height: 30px;
  border: none;
  background: #3475ab;
  border-radius: 5px;
  color: white;
}
</style>
