
<template>
  <div class="component-frame">
    <slot />
  </div>
</template>

<script>
export default {
  name: "ComponentFrame",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.component-frame {
  border: 3px solid #c1c1c1;
  border-radius: 5px;
  padding: 10px;
}
</style>
