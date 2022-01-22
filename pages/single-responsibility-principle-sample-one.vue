<template>
  <div>
    <ComponentFrame>
      <SingleResponsibitliyPrincipleBadInput
        label="First name"
        labelColor="#303030"
        inputPlaceholder="Please enter your first name"
        buttonText="Confirm"
        @textChange="handleTextChange"
        @buttonClick="handleButtonClick"
      />
    </ComponentFrame>
    <ComponentFrame>
      <SingleResponsibitliyPrincipleGoodLabel
        text="First name"
        color="#303030"
      />
      <SingleResponsibitliyPrincipleGoodInput
        placeholder="Please enter your first name"
        :style="{ marginTop: '7px' }"
        @input="handleTextChange"
      />
      <SingleResponsibitliyPrincipleGoodButton
        text="Comfirm"
        :style="{ marginTop: '4px' }"
        @click="handleButtonClick"
      />
    </ComponentFrame>
  </div>
</template>

<script>
export default {
  methods: {
    handleTextChange() {
    },
    handleButtonClick() {
    },
    handleSubmit() {
    },
  },
}
</script>
