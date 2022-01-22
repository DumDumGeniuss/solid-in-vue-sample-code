
<template>
  <div class="good-button">
    <button @click="handleClick">{{text}}</button>
  </div>
</template>

<script>
export default {
  name: "GoodButton",
  props: {
    text: String,
  },
  methods: {
    handleClick() {
      this.$emit('click');
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.good-button {
  display: flex;
}
.good-button button {
  width: 100%;
  height: 30px;
  border: none;
  background: #3475ab;
  border-radius: 5px;
  color: white;
}
</style>
